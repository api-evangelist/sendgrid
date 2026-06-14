# SendGrid GraphQL

## Title
SendGrid Conceptual GraphQL Schema

## Description
SendGrid (Twilio) is a REST-only email delivery platform — it does not expose a native GraphQL endpoint. This schema is a conceptual translation of the SendGrid email data model into GraphQL SDL, derived from the official REST API reference at https://docs.sendgrid.com/api-reference. It covers the full surface area of SendGrid's email sending, marketing campaigns, contact management, suppression, authentication, statistics, and webhook capabilities.

Use this schema for:
- Code generation tooling that targets SendGrid's REST API
- API gateway or BFF (backend-for-frontend) layers that wrap SendGrid in GraphQL
- Documentation and exploration of SendGrid's data model
- Type-safe client generation

## Endpoint
None — SendGrid does not offer a GraphQL endpoint. All production API calls use the REST API at `https://api.sendgrid.com/v3/`.

## Documentation
- API Reference: https://docs.sendgrid.com/api-reference
- Mail Send: https://www.twilio.com/docs/sendgrid/api-reference/mail-send
- Marketing Campaigns: https://www.twilio.com/docs/sendgrid/api-reference/contacts
- Suppressions: https://www.twilio.com/docs/sendgrid/api-reference/suppressions-unsubscribe-groups
- Templates: https://www.twilio.com/docs/sendgrid/api-reference/transactional-templates
- Statistics: https://www.twilio.com/docs/sendgrid/api-reference/stats
- Webhooks: https://www.twilio.com/docs/sendgrid/api-reference/webhooks

## Schema Source
Conceptual — derived from the SendGrid REST API surface (OpenAPI specifications in the `openapi/` directory of this repository).
