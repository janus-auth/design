# Introduction

Janus is an authentication and authorization system with the following properties:

- **Provable**: It's always possible to prove the correctness of a statement. [1]() [2]() [3]()
- **[Antifragile](https://en.wikipedia.org/wiki/Antifragility)**: As load increases, the system becomes more robust.
- **Federated**: It's possible to federate multiple instances, thanks to 
its [capability](https://en.wikipedia.org/wiki/Capability-based_security) based model.

This is the repository for the design documents. Use the table of contents below to navigate, or visit:
-  [Javascript implementation](https://github.com/janus-auth/janus.js) of client and server.
-  [Rust implementation](https://google.com) (coming soon)
-  [Youtube channel](https://www.youtube.com/channel/UC7i6ZGtI2b2XA5n2lgwNkaQ) where we discuss about the Janus system.

## Table of contents
- [Introduction](docs/10_introduction/README.md) 
  - [Problem](docs/10_problem/README.md): What problems does Janus try to solve?
  - [Solution](docs/10_introduction/20_solution/README.md): How does Janus solves these problems?
- [Architecture](docs/20_architecture/README.md): What is Janus made of?
- [Protocols](docs/30_protocols/README.md): How does Janus work?


## TODOS

- profiles and downgrade attacks
- web crypto api
- wasi crypto api
- hardware tokens
