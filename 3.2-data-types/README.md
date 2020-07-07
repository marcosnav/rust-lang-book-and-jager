# 3.2 Data Types

There are various data types, more can be seen in [here](https://doc.rust-lang.org/book/ch03-02-data-types.html).

Type declaration examples:
```rust
let y: f32 = 3.0; // Floating point
let f: bool = false; // Boolean
```

## Char
```rust
let c = 'z'; // char (four bytes in size)
```

## Tuples
```rust
let tup = (500, 6.4, 1);
let tup: (i32, f64, u8) = (500, 6.4, 1);
```

## Arrays
In contrast with tuples, arrays must have the same type for all values.
```rust
let a = [1, 2, 3, 4, 5];
let a: [i32; 5] = [1, 2, 3, 4, 5];

let first = a[0];
let second = a[1];
```

## Numeric operations
```rust
fn main() {
    // addition
    let sum = 5 + 10;

    // subtraction
    let difference = 95.5 - 4.3;

    // multiplication
    let product = 4 * 30;

    // division
    let quotient = 56.7 / 32.2;

    // remainder
    let remainder = 43 % 5;
}
```
