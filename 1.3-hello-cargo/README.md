# 1.3 Resume

Cargo is Rust’s build system and package manager. It helps on:
- building your code, 
- downloading the libraries your code depends on, 
- building those libraries
- but more importantly, as a convention!

### Creating new projects with cargo:

`$ cargo new hello_cargo`

Above command creates a new dir hello_cargo containing:
- `Cargo.toml` to contain the package details and dependencies
- `src` dir with the entry file `main.rs`

### Building and Running a Cargo Project
Located in the project dir.

Build:
`$ cargo build`

The above command creates a `target/debug/hello_cargo`

Run: 
`$ ./target/debug/hello_cargo`

Building a project creates a `Cargo.lock` that is nothing more than a lock file to keep track of the exact versions of dependencies in your project.

**Build and run with one command!**
`$ cargo run`

Check for possible compiling issues without building a binary:
`$ cargo check`

### Build for release
This command will create an executable with some optimizations in target/release instead of target/debug.

`$ cargo build --release`
