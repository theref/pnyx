# Pnyx

> The hill in Athens where citizens gathered to debate and vote. The birthplace of democracy.

**Pnyx** (pronounced "niks") is a censorship-resistant discussion platform built on [ForumMagnum](https://github.com/ForumMagnum/ForumMagnum).

## What is Pnyx?

A discussion platform where:

- **Real identity required** — Government ID verification at signup. All posts display your first name, surname initial, and nationality (e.g., "John S., United Kingdom")
- **Permanent record** — Daily backups to [Arweave](https://arweave.org) create an immutable, public archive
- **Forkable** — Anyone can restore the full platform from any backup point
- **Self-hostable** — Run your own instance with standard infrastructure

## Core Principles

1. **Identity as commitment** — Accountability through verified identity
2. **Permanence** — Content survives forever on Arweave
3. **Transparency** — Full database backups are public (users informed at signup)
4. **Forkability** — Community disputes? Fork from any backup

## Tech Stack

- **Frontend**: TypeScript, React
- **Database**: MongoDB
- **Identity**: Government ID verification (Jumio/Onfido/Persona)
- **Storage**: Arweave via Irys
- **Discovery**: ENS record pointing to latest backup

## Privacy Model

Users are informed at signup:

- Your verified name and nationality are displayed on all posts/comments
- All content is backed up permanently to Arweave
- Backups are public and immutable - this cannot be undone
- Email addresses are NOT included in backups
- Account recovery is via ID re-verification

## Development

This project uses **bd** (beads) for issue tracking:

```bash
bd ready              # Find available work
bd show <id>          # View issue details
bd update <id> --status in_progress
bd close <id>
```

See [AGENTS.md](./AGENTS.md) for development workflow.

## License

**GPLv3** — Forked from ForumMagnum. Pnyx must remain open source.

## Status

Early development. See issue tracker for current progress.
