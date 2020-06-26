# 2 Resume

A simple guessing game...

At the very top of `main.rs` we bring a library to obtain user input:
`use std::io;`

The `io` library comes from the standard library (which is known as `std`).

### Comments in Rust
`// immutable`

### Variables

`let mut guess = String::new();`

Rundown:
- `let` statement is used to create a variable
- In Rust, variables are immutable by default
- Use `mut` before the variable name to make a variable mutable
- `String::new()` returns a new instance of type `String` (UTF-8 encoded bit of text)
- The `::` syntax in `::new` indicates that `new` is an associated function of the `String` type


### stdin
```
io::stdin()
  .read_line(&mut guess)
```

Rundown:
- The `std::io::stdin` returns a handle to the standard input for the terminal
- `read_line` reads the given input
- The `&` indicates that this argument is a reference
- References are immutable by default. Hence, the need to `&mut guess` rather than `&guess` to make it mutable

### The `Result` type:
The `Result` types are enumerations (`enums`). The variants are `Ok` or `Err`.

```
.expect("Failed to read line");
```

The `.expect` function returns an instance of `io::Result`

### Printing with placeholders
In this next line, `{}` is a placeholder to be replaced with the `guess` variable value.
`println!("You guessed: {}", guess);`

Another example:
```
let x = 5;
let y = 10;
println!("x = {} and y = {}", x, y);
```
Would print `x = 5 and y = 10`.
