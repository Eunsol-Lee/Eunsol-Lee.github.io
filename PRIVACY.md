# Privacy Policy — atlas

atlas is a personal automation toolkit operated by Eunsol Lee. It synchronizes
data from external APIs (Gmail, Google Calendar, Google Drive, Slack, Notion,
GitHub) into a local PostgreSQL database for the operator's private use.

## Data we access

When the operator authorizes a Google account via OAuth 2.0, atlas reads:

- `https://www.googleapis.com/auth/gmail.readonly` — read-only Gmail messages
- `https://www.googleapis.com/auth/calendar.readonly` — read-only Calendar events
- `https://www.googleapis.com/auth/drive.readonly` — read-only Drive files

These are used only to synchronize data into the operator's local database.
atlas does not send mail, modify calendar events, or change files.

## How we store data

- OAuth refresh tokens are stored in a local `.env` file on the operator's
  machine. They are never transmitted to third parties.
- Synchronized data is stored in a local PostgreSQL database running on the
  operator's own hardware.
- No data is uploaded to remote servers operated by atlas.

## How we share data

- atlas does not share data with third parties.
- atlas does not collect analytics, telemetry, or usage statistics.

## How to revoke access

The authorized account can revoke atlas's access at any time:

1. Visit https://myaccount.google.com/permissions
2. Locate the atlas OAuth client and click "Remove access"

Once revoked, the next sync attempt will fail with `invalid_grant`.

## Contact

Eunsol Lee — eunsol@medibloc.org

Last updated: 2026-05-20
