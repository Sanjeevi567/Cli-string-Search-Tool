# Cli-string-Search-Tool

# This is a small project in Rust but demonstrates a lot of good practices in software development.

## Modular

Each component is independent of the other. All parallel iterators are implemented in the par library. We use reuse them other than this project. The internal 
details are not exposed to the client. All the codes are single-threaded by default, which means they are extensible to other concurrency models that would be faster than default implementation.

## Embrace the DRY(Don't Repeat Yourself)

Crates.io have a lot of libraries to avoid the much more boilerplate code without more effort.

## Productivity
Cargo takes care of downloading and compiling the dependencies for you. Cargo can do a lot more than just manage dependencies. We can cross-compile the code to other platforms. Cargo check command to reduce the compile time, cargo run to check the result, and cargo build --release to release the executable with more optimization which takes more time than previous cargo commands. We can see the documentation of the crate we downloaded without an internet connection.

## Testing
Cargo already supports unit testing and an integrated testing framework. Testing is simple as writing test functions and testing them via cargo test.

## Documentation
We can document the code as we write and generate them as HTML via cargo doc.

## Robust
Because we get the inputs from the user via the command line it's essential to be robust to the errors. Rust makes this easy, we can't forget to handle the error.

## Concurrency
Because of rust fearless concurrency, we can introduce concurrency from the start to increase the performance without worry about race conditions and other common mistakes you see in another language which must take more time.

## Distribution
This project is written in Rust we can easily share the executable without installing Rust which means there is no runtime needed to run the executable unlike
dynamic programming language where the runtime is always needed to run them.
