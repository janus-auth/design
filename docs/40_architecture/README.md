# Architecture

This section describes the components which makes up the architecture of the Janus system.

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

```mermaid
flowchart LR

  id1 --- auth
  id1 --- id4 --- sid1

  subgraph auth [auth-services]
    direction LR
    sid1
    sid2
    sid3
  end

  subgraph dmz [DMZ]
    auth --- id2
    auth --- id3 --- id2
    auth --- sid4
    id2 --- sid5 --- id3
  end


  sid1[identity-service]
  sid2[session-service]
  sid3[capability-service]
  sid4[hsm-service]
  sid5[analytic-service]

  id1[Clients]
  id2[(DataStore)]
  id3(EventBus)
  id4(Providers)
```

- Services
  - [auth-service](10_auth-service.md)
  - [hsm-service](20_hsm-service.md)
  - [identity-services](30_identity-services.md)
  - [DataStore](40_DataStore.md)
  - [EventBus](50_EventBus.md)
- [Providers](20_identity-services/20_providers.md)
- [Profiles](10_auth-service/30_profiles.md)
