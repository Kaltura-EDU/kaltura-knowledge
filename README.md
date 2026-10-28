# kaltura-knowledge

Community-maintained knowledge, troubleshooting tips, and best practices for Kaltura in education.

This is a place for the Kaltura-EDU community to write down what we learn: API quirks, configuration lessons, support fixes, and workarounds. It is a companion to [api-scripts](https://github.com/Kaltura-EDU/api-scripts), which holds working scripts for the Kaltura API.

## Read this first: how much to trust what you find here

Not everything here is guaranteed to be true for your environment. Every note carries a `status` field:

| Status | Meaning |
|---|---|
| **Unverified** | Someone reported or observed this. It may be correct, but nobody has independently confirmed it. |
| **Confirmed** | Verified by testing, Kaltura documentation, or Kaltura support, and the note says how. |
| **Disputed** | Contributors have seen conflicting results. |
| **Outdated** | Was true for an older version or setup. Kept for context. |

Kaltura behavior also varies by version, product (KMC, KAF, MediaSpace, REACH), and institution settings. Check the `environment` field and test before relying on a note in production.

## What's in the repo

| Folder | Contents |
|---|---|
| [`notes/`](notes) | Curated knowledge notes, organized by topic |
| [`meetings/`](meetings) | AI-generated summaries of community meetings. These are conversation, not guidance. |
| [`templates/`](templates) | The knowledge note template |

## Getting involved

- **Add or improve a note:** see [CONTRIBUTING.md](CONTRIBUTING.md).
- **Ask a question or start a conversation:** use [Discussions](../../discussions).
- **Using an AI assistant?** Point it at this repo. [AGENTS.md](AGENTS.md) tells it how notes are structured and what it must not claim.

## Please don't post

Passwords, API secrets, session tokens (KS), partner IDs tied to your institution, internal URLs, or personal information about students, staff, or vendors. See [CONTRIBUTING.md](CONTRIBUTING.md#what-not-to-include).
