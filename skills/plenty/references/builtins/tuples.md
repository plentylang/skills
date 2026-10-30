<!-- Copied from the Plenty 0.7.1 book page book/src/design/facilities/01-builtins/tuples.md. Edit the book, not this copy. -->

# Tuple operations

Tuples provide fixed component access with a nonnegative integer literal index.
Construction, indexing, unpacking, and component-loan rules are defined in
tuple types.

Supported tuples compare structurally without allocation. [copy](construction-copy.md)
duplicates copyable components and mutable contents fallibly;
[formatting](formatting.md) displays supported component values. Types containing
stored recursive data are excluded from these automatic traversals.

A tuple can store concrete owned callbacks of different types. Reusable calls
borrow their indexed component; consuming calls require extraction by unpacking.
See stored callable values.
