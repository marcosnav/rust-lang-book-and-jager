# 3.5 Control Flow

## `if` expressions

```rust
fn main() {
  let number = 3;

  if number < 5 {
    println!("less than 5");
  } else if number > 10 {
    println!("too much! more than 10");
  } else {
    println!("ok");
  }
}
```

Unlike other languages like Ruby and JS, Rust doesn't try to convert non-Boolean types to a Boolean. The following example results in an error.

```rust
if number {
  println!("number was three");
}
```

## `let` in an `if` statement

```rust
// Possible values should be of same type
let number = if condition { 5 } else { 6 };

// This statement errors due to incompatible types (number and string)
let number = if condition { 5 } else { "six" };
```

## Loops

The following program would repeat until stopped manually. (Ctrl + C)

```rust
fn main() {
  loop {
    println!("again!");
  }
}
```

```rust
// Returning values from loops
// When counter gets to 10, result = 20
let result = loop {
  counter += 1;

  if counter == 10 {
    break counter * 2;
  }
};
```

## Conditional loops `while`

```rust
while number != 0 {
  println!("{}!", number);

  number -= 1;
}
```

## Loop through collection with `for`

```rust
let a = [10, 20, 30, 40, 50];

for element in a.iter() {
  println!("the value is: {}", element);
  // the value is: 10
  // the value is: 20
  // ...
}
```

```rust
// Countdown with the .rev method
for number in (1..4).rev() {
  println!("{}!", number);
  // 4
  // 3
  // ...
}
```
