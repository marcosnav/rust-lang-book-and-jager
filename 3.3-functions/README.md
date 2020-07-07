# Functions

```rust
fn main() {
  println!("Hello, world!");
  another_function();
}

fn another_function() {
  println!("Another function.");
}
```

## With Parameters
```rust
fn another_function(x: i32, y: i32) {
  println!("The value of x is: {}", x);
  println!("The value of y is: {}", y);
}
```

## Statements and blocks
```rust
fn main() {
  let x = 5;

  let y = {
    let x = 3;
    x + 1
  };

  println!("The value of y is: {}", y);
}
```

```rust
// In the previous code,
// this is a block that handles its own internal statements and bounds the value of 4 to "y"
{
  let x = 3;
  x + 1
};
```

## Functions with return values
The returned value type must be declared after an arrow.

```rust
fn main() {
  let x = plus_one(5);
  println!("The value of x is: {}", x);
}

fn plus_one(x: i32) -> i32 {
  // Error would show by changing it from an expression to a statement adding a semi-colon
  x + 1
}
```

Returned values shouldn't be followed by `;` semi-colons.
