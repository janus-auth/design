# Architecture

This section describes the components which makes up the architecture of the Janus system.

- [auth-service](10_auth-service.md)
- [hsm-service](20_hsm-service.md)
- [identity-services](30_identity-services.md)
- [DataStore](40_DataStore.md)
- [EventBus](50_EventBus.md)

```mermaid
flowchart LR

    id1 --- sid1

    subgraph dmz [Demilitarized Zone]
        sid1 --- id3
        sid1 --- sid2
        sid1 --- sid4 --- id3
        sid1 --- sid3
    end

    sid1[auth-service]
    sid2[hsm-service]
    sid3[identity-services]
    sid4(EventBus)

    id1[Clients]
    id3[(DataStore)]
```
