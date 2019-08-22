# DANAA
Dynamic Assets Names Autonomous Agent  (for Obyte)

## Use cases:
Let you register a nicer name for your assets.
* Add a new entry: set at minimum: 'unit_id', 'shortName', 'ticker' and 'decimals';
* Change one of your exisiting entries: set at minimum: 'unit_id', 'shortName', 'ticker' and 'decimals';
* Get the nice name from another aa: var["<DANAA_address>"][<asset id>_shortName];

## State variables
* <unit_id>_shortName: contains the new_name and can be used by other AA to show this nice name;
* <unit_id>_issuer: address of the user that issued the asset; we have to trust the address that register the asset to be the issuer as we cannot access any field of an units;
* <unit_id>_ticker: ticker choosen to represente the asset;
* <unit_id>_decimals: number of decimal possible with this asset;
optionals:
* <unit_id>_name: full name of the asset, by default concatenation of shortName and Issuer;
* <unit_id>_description: short description, by default "Asset called +$shortName+ issued by +$issuer+, with +$decimals+ decimals available. Its ticker is +$ticker+ and it is defined by the unit '+$unit_id+'."

## TODO
* In the future if it possible to access the fields of an unit, we could allow only the author of the asset unit to be able to choose a name for its asset.

