# Rust-Axum-Intro

This is a rust project that uses the axum framework to create a simple web server.

The main reason to make this little projecto is to learn how to use the axum framework and to have a simple example to use as a reference in the future.

Have for sure this is an example taken from the youtube channel of [Jeremy Chone](https://www.youtube.com/watch?v=XZtlD_m59sM&t=2320s), A real good example to start with axum.

**Note:** I am a rust beginner, and I don't have any experience with the axum framework, so must of the thing Jeremy just did I didn't understand it, but keep going the start is always the hardest part.

## How to run the project

To run the project is key to have the rust Binary crate cargo-watch installed, if you don't have it installed you can install it by running the following command:

```bash
cargo install cargo-watch
```

To run the project you can run the following command:

```bash
cargo watch -q -c -w ./src -x run
```

To run the tests you can run the following command:

```bash
cargo watch -q -c -w ./src -x "test -- --nocapture"
```

In case you have a windows machine is important to know that every time a exe file is being executed this file is locked by the system, so if you want to run the project in a windows machine you need to run it in different profile, or just run it in the --release mode.

```bash
cargo watch -q -c -w ./src -x "test --release -- --nocapture"
```
