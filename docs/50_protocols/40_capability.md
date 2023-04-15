# Introduction

## Sign

Hello

```json
{
  "request": {
    "target": "string",
    "method": "string", 
    "body": "string"
  },
  "session": {
    "sessionId": "uuid",
    "timestamp": "date",
    "nonce": "string"
  },
  "hash": "string",
  "signature": "string"
}
```

## Attest

Prove the correctness of a capability token, equivalent to the verify in asymmetric cryptography.

## Accredit

Forge a capability token, equivalent to the sign in asymmetric cryptography.

Result:

```json

{
  "token": {
    "instanceId": "uuid",
    "identityId": "uuid",
    "capability": "string"
  },
  "hash": "string",
  "signature": "string"
}

```
