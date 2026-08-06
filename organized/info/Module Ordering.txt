Modules are ordered in a depth-first search starting from the weapon/body/gadget
and searching up, right, down, then left.

In pseudocode, the process is:

```
module_list = new list

Function gather_data:
    Input: current_module

    If current_module is powered:
        Add current_module to module_list

    If module above current_module exists and has connection:
        Run gather_data on module above current_module

    If module right of current_module exists and has connection:
        Run gather_data on module right of current_module

    If module below current_module exists and has connection:
        Run gather_data on below of current_module

    If module left of current_module exists and has connection:
        Run gather_data on module left of current_module
```

Where to start the process, run `gather_data` on one of the ship's
weapons, gadgets, or body.

Some examples of module ordering in action using images:

Note the "and has connection" part of the ordering, as disconnecting a path
between two modules can radically change the resolution order:
