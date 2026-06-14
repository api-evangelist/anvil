# Anvil GraphQL API

The Anvil GraphQL API is the primary query and mutation interface for the Anvil platform. It exposes the full range of Anvil's document automation capabilities, including e-signature packet management (EtchPackets), workflow orchestration (Welds), webform configuration (Forges), PDF template management (Casts), webhook subscriptions, and user/organization administration. The API supports 10 named queries and over 40 mutations, giving developers complete programmatic control over all Anvil resources.

Authentication is performed using HTTP Basic Auth with your Anvil API key as the username and an empty password, or by passing the API key as a Bearer token in the Authorization header. All requests must be POST requests with a `Content-Type: application/json` header. File uploads larger than 1MB must use multipart form encoding as specified by the GraphQL multipart request specification.

The schema is downloadable in SDL format via a GET request to `https://app.useanvil.com/graphql/sdl` (requires authentication). Core object types include User, Organization, Weld (Workflow), Forge (webform), Cast (PDF template), WeldData (workflow submission), Submission, EtchPacket, EtchTemplate, DocumentGroup, Signer, SignerToken, Webhook, WebhookAction, and WebhookLog, with corresponding pagination types for each.

**Endpoint:** https://graphql.useanvil.com

**Documentation:** https://www.useanvil.com/docs/api/graphql/

**References:**

- Documentation: https://www.useanvil.com/docs/api/graphql/
- GettingStarted: https://www.useanvil.com/docs/api/getting-started/
