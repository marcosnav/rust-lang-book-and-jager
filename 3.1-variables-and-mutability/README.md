# 3.1 Variables

```rust
let x = 5; // Immutable
x = 10; // Error, cannot assign twice to immutable variable

let mut y = 20; // "mut" allows for mutability
y = 25; // OK
```

Being unable to change the value of a variable is similar to another programming concept that most other languages have: constants.

Anyway, in Rust there are a few differences between constants and variables.

- Constants aren’t just immutable by default—they’re always immutable.
- You declare constants using the const keyword instead of the let keyword, and the type of the value **must** be annotated.

```rust
const MAX_POINTS: u32 = 100_000;
```
