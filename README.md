# Identity & Security TypeScript POC

A TypeScript/Node.js proof of concept exploring secure identity
and API authentication patterns.

## Focus Areas

- OAuth 2.0 concepts
- OpenID Connect
- JWT validation
- JWS signatures
- JWKS-based key discovery
- Token expiration validation
- Issuer validation
- Audience validation
- JTI validation
- Authentication middleware
- Secure HTTP headers
- Replay protection concepts
- API authorization

## Technology

- TypeScript
- Node.js
- Express.js
- JWT
- JWK / JWKS
- REST APIs

## Architecture

Client
   |
   v
Authentication / Identity Provider
   |
   v
JWT / ID Token
   |
   v
Node.js API
   |
   +--> Signature validation
   +--> Issuer validation
   +--> Audience validation
   +--> Expiration / TTL validation
   +--> JTI validation
   +--> Authorization
   |
   v
Protected API

## Security Considerations

The implementation demonstrates validation of:

- Token signature
- Issuer
- Audience
- Expiration
- Token ID
- Required claims

The project is intended as a technical demonstration and does
not contain production credentials or client-specific code.
