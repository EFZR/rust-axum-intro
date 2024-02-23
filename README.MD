# 🦀 Rust-Axum-Intro 🕸️

This is a Rust project that uses the Axum framework to create a simple web server. 🌐

The main purpose of this little project is to learn how to use the Axum framework and to have a simple example to use as a reference in the future. 📚

This example is taken from the YouTube channel of [Jeremy Chone](https://www.youtube.com/watch?v=XZtlD_m59sM&t=2320s). It's a really good starting point for learning Axum. 🎥

**Note:** I am a Rust beginner, and I don't have any experience with the Axum framework. Most of the things Jeremy did, I didn't fully understand, but I'm pushing forward. The start is always the hardest part. 💪

## 🚀 How to run the project

To run the project, you need to have the Rust binary crate `cargo-watch` installed. If you don't have it installed, you can install it by running the following command:

```bash
cargo install cargo-watch
```

To run the project, use the following command:

```bash
cargo watch -q -c -w ./src -x run
```

To run the tests, use the following command:

```bash
cargo watch -q -c -w ./tests -x "test -- --nocapture"
```

🖥️ For Windows users: It's important to know that every time an .exe file is being executed, this file is locked by the system. So, if you want to run the project on a Windows machine, you need to run it in a different profile, or just run it in the --release mode.

```bash
cargo watch -q -c -w ./tests -x "test --release -- --nocapture"
```
