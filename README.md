# SMS Inbox (Inbound Webhook)

This is a small internal tool that receives inbound SMS messages via webhooks
(e.g., from Twilio) and displays them in a simple inbox for operational/support
communication.

## What it does
- Receives inbound SMS to SMS-capable phone numbers
- Twilio sends an HTTPS webhook (HTTP POST) to the server
- The server stores messages in a simple JSON inbox for development/testing
- No marketing, no bulk messaging, no unsolicited traffic

## Intended usage
- Inbound SMS only (primary)
- Optional low-volume transactional messages (if needed), only to users who request/consent

## Data handling
- For development: stores inbound messages in a JSON file
- Sensitive data should be redacted in logs/screenshots

## Screenshots
The screenshots below show a development setup where an inbound SMS webhook is received by the server and stored in a simple JSON inbox. URLs/tokens are redacted for security.
![Server logs](screenshots/logs.png)
![Inbox output](screenshots/inbox.png)
