# auth-service

The auth-service is responsible for authenticating users and issuing JWTs. 

```mermaid
flowchart LR

    Client --- id1

    subgraph "auth-service"
        id1 --- id2 --- id3
        id1 --- id4
    end

    id1(Worker)
    id2(DataStore)
    id3(Cache)
    id4(KeyStore)
```


## Handlers

System Handlers:
- Canary
- Time
- Health

Identity Handlers:
- Join
- Rotate
- Leave

Session Handlers:
- Login
- Logout

Capability Handlers:
- Attest
- Accredit
