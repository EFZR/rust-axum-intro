# 🦀 Rust-Axum-Intro 🕸️

This is a Rust project that uses the Axum framework to create a simple web server. 🌐

The main purpose of this little project is to learn how to use the Axum framework and to have a simple example to use as a reference in the future. 📚

This example is taken from the YouTube channel of [Jeremy Chone](https://www.youtube.com/watch?v=XZtlD_m59sM&t=2320s). It's a really good starting point for learning Axum. 🎥

**Note:** I am a Rust beginner, and I don't have any experience with the Axum framework. Most of the things Jeremy did, I didn't fully understand, but I'm pushing forward. The start is always the hardest part. 💪

## 🛠 Project Overview

This project is a simple but complete web server built with the Axum framework. Here's a breakdown of its main components:

- `main.rs`: This is the main file where the server is created and routes are defined.

- `model.rs`: This file defines the `Ticket` data model. The server can create, read, and delete tickets.

- `log.rs`: This file sets up a comprehensive logger. It logs the request and response details of the server, including UUID, timestamp, request path, request method, user ID, client error type, error data, and error type.

- `error.rs`: This file defines the error types used in the project and handles error scenarios.

- `ctx.rs`: This file defines the context struct. It's used to check if a user is authenticated.

- `web/mw_auth.rs`: This file defines the authentication middleware. It includes:
  - The `Ctx` extractor, used to check user authentication and retrieve user data.
  - `mw_ctx_resolver`, used to resolve the `Ctx` extractor.
  - `mw_require_auth`, used to verify user authentication.

- `web/routes_login.rs`: This file defines the routes for user login and logout.

- `web/routes_ticket.rs`: This file defines the routes for creating, reading, and deleting tickets.

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
