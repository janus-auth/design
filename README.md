# Introduction

Janus is an authentication and authorization system with the following properties:

- **Provable**: It's always possible to prove the correctness of a statement. [1]() [2]() [3]()
- **[Antifragile](https://en.wikipedia.org/wiki/Antifragility)**: As load increases, the system becomes more robust.
- **Federated**: It's possible to federate multiple instances, thanks to 
its [capability](https://en.wikipedia.org/wiki/Capability-based_security) based model.

This is the repository for the design documents. Use the table of contents below to navigate, or visit:
-  [Javascript implementation](https://github.com/janus-auth/janus.js) of client and server.
-  [Rust implementation](https://google.com) (coming soon)
-  [YouTube channel](https://www.youtube.com/channel/UC7i6ZGtI2b2XA5n2lgwNkaQ) where we discuss the Janus system.

## Table of contents
[Introduction](docs/00_introduction/README.md): What problems does Janus try to solve, and how?

**Problems**: What problems does Janus try to solve?
- [Secrets](docs/10_problems/10_secrets.md): What problems does Janus try to solve, and how?
- [Fragility](docs/10_problems/10_secrets.md): What problems does Janus try to solve, and how?
- [Fragmentation](docs/10_problems/10_secrets.md): What problems does Janus try to solve, and how?
- [Attacks](docs/10_problems/10_secrets.md): What problems does Janus try to solve, and how?
**Solutions**: How does Janus solve the auth problem?
- [Hybrid cryptosystems](docs/20_solutions/10_hybrid.md)
- [Scalability](docs/20_solutions/10_hybrid.md)
- [Capabilities](docs/20_solutions/10_hybrid.md)
- [Defenses](docs/20_solutions/10_hybrid.md)

**Tools**: Which tools does Janus use?
- [Crypto primitives](docs/30_tools/10_crypto.md)
- [Janus micro](docs/30_tools/50_micro.md)

[Architecture](docs/40_architecture/README.md): What is Janus made of?
- [Auth service](docs/40_architecture/10_auth-service/10_auth-service.md)
- [Identity service](docs/40_architecture/20_identity-services/10_identity-services.md)
- [HSM service](docs/40_architecture/30_hsm-service/10_hsm-service.md)
- [DataStore](docs/40_architecture/40_DataStore/10_DataStore.md)
- [Event Bus](docs/40_architecture/50_EventBus/10_EventBus.md)


[Protocols](docs/50_protocols/README.md): How does Janus work?

## TODOS

- permission tree
- authorization flow
- blockchain storage