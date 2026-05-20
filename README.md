# atlas

Personal automation toolkit by Eunsol Lee. atlas is a collection of small data
sync and analysis scripts that run on a personal Mac to keep external service
data (Gmail, Calendar, Drive, Slack, Notion, GitHub) mirrored in a local
PostgreSQL database for offline analysis and AI-assisted workflows.

## Components

- **data-bridge** — syncs external API data into local PostgreSQL.
- **atlas** — analysis layer over the synced data; produces daily briefings
  and answers questions.

## Privacy

All data accessed by atlas stays on the operator's local hardware. atlas
does not transmit user data to third parties.

See the full [Privacy Policy](./PRIVACY.html).

## Contact

Eunsol Lee — eunsol@medibloc.org
