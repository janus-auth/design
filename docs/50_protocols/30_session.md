# Session protocols
details
## Login

The login event is used to negotiate a new session token on
a device that was never used before:

```mermaid
sequenceDiagram

   participant C as Client
   participant I as Instance
   participant P as Provider

   C->>I: Login request (1)
   alt Route challenge via provider (2)
      I->>P: 
      P->>C: 
   end
   C->>I: Signed response (3)
   I->>C: Session token (4)
```

A session token looks like this:
```json
{
  "identityId": "uuid",
  "providerId": "uuid",
  "sessionId": "uuid",
  "timestamp": "date",
  "key": "spki",
  "secret": "base64",
  "signature": "base64"
}
```

## Refresh

The refresh event is used to refresh a session token in case
the client 

```mermaid
sequenceDiagram

   participant C as Client
   participant I as Instance

   C->>I: Refresh request (1)
   I->>C: Session token (2)

```

## Logout

The logout event is used to delete a session

## View

The view event is used to query for the details of a session.


