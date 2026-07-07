To enforce modularity in a monolith architecture: 

1: One responsibility per module
    -Example: Users, Orders, Payments, Inventory.
    -Each owns a distinct business domain.

2: Clear public interfaces
    -Other modules interact only through exposed APIs/functions.
    -Don't access another module's internal classes or data directly.

3: Hide implementation details
    -Keep helper classes/functions private to the module.
    -Expose only what's necessary.

4: Dependency direction
    -Define which modules are allowed to depend on which.
    -Avoid circular dependencies (A → B → A).
    -Write this explicitly in notes for a section beforehand

5: Thin glue code
    -Top-level code wires modules together.
    -Business logic stays inside the modules.

6: Independent tests
    -Most tests should exercise a single module.
    -Integration tests verify modules work together.

7: Separate folders/packages
    -Organize by feature rather than by file type.


Use architecture enforcement tools to enforce modularity principles automatically, can automatically enforce:
    -No circular dependencies
    -Rules about what modules a module can use
    -Only public APIs can be used
    -Layers only depend downward (for example: UI -> Service -> Data)
    -No cross-module access to internal files

