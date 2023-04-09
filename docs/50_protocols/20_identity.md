# Identity protocol

## Join

The join event is used to create a new identity.

- [Client]: Resolve root certificate
- [Client]: Generate keypair
- [Client]: Request service
- [Server]: Respond with certificate chain
- [Server]: Respond with challenge
- [Client]: Solve challenge
- [Server]: Verify challenge
- [Server]: Respond with capability token

## Leave

The leave event is used to delete an identity.

## Rotate

The rotate event is used to rotate the keypair of an identity.

## View

The view event is used to view the certificates associated with an identity.
