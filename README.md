# DANAA
Dynamic Assets Names Autonomous Agent  (for Obyte)

## Use cases:
Let you register a nicer name for your assets.
* Add a new entry: set 'unit_id' and 'new_name';
* Change one of your exisiting entries: set 'unit_id' and 'new_name';
* Get the nice name from another aa: var["M2GL3REJ3TJPHVC4GMCBKQI54NEKRYNH"][<asset id>]

## State variables
* <unit_id>: contains the new_name and can be used by other AA to show this nice name;
* <unit_id>_author: address of the user that create the entry;

## TODO
* In the future if it possible to access the fields of an unit, we could allow only the author of the asset unit to be able to choose a name for its asset.

