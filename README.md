# Cli-string-Search-Tool

# This is a small project in rust but demonstrate the lot of good practices in software development.

## Modular

Each componets are independent of each other.All parallel iterators are implement in the par library.We use reuse them other than this poject.The internal 
details are not exposed to the client.All the codes are single threaded by default,which means they are extensible to other concurrency models you that would faster than default implementation.

## Embrace the DRY(Don't Repeat Yourself)

Crates.io have lot of libraries to avoid the much more boilerplate code without more effort.

## Productivity
Cargo take care of downloading and compiling the dependencies for you.Cargo can do lot more than just managing dependencies.We can cross compile the code to other platforms.Cargo check command to reduce the compile time ,cargo run to check the result ,cargo build --release to release the executable with more optimization which takes more time than previous cargo commands.

## Testing
Cargo already supports unit testing and integrated tesing framwork.Testing is simple as writting test function and test them via cargo test.

## Documentation
We can document the code as we write and generate them as html via cargo doc.

## Robust
Because we get the inputs from the user via cli it's essential to robust to the errors.Rust make this easy,we can't forgot to handle the error.

## Concurrency
Because of rust fearless concurrency, we can introduce concurrency from the start to increase the performance without worry about race condtion and other common mistakes you see in other langauge which must be take more time.

## Distribution
This project written in rust we can easily share the executable without installing rust which means there is no runtime needed to run the executable unlike
dynamic programming language where the runtime is always needed to run them.
