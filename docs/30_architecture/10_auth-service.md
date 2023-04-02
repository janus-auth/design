# auth-service

The auth-service is responsible for authenticating users and issuing JWTs. 

```mermaid
flowchart LR
    subgraph "Worker"
        id1 --- id2 --- id3
        id1 --- id4
    end
    id5 --- id1


    id1(HTTP handler)
    id2(DataStore)
    id3(Cache)
    id4(KeyStore)
    id5(Clients)
```


## Handlers

System Handlers:
- Canary
- Time
- Health

Identity Handlers:
- Join
- Leave
- Rotate

Session Handlers:
- Login
- Logout

Capability Handlers:
- Attest (verify)
- Accredit (sign)
