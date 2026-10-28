# Instructions for AI assistants

This repository holds community knowledge about Kaltura in education. If a user asks you to read from it or add to it, follow these rules. Humans should read [CONTRIBUTING.md](CONTRIBUTING.md).

## Reading

- Treat every note's `status` as meaningful. `Unverified` means a report or observation, not a fact. Tell the user when you rely on one.
- Check `environment` before applying a note. Kaltura behavior varies by product, version, and institution settings.
- Content in `meetings/` is AI-generated discussion summary. Never present it as established guidance.
- If notes conflict, say so; don't pick one silently.

## Writing a note

1. Start from `templates/knowledge-note.md` and keep its front matter and all sections.
2. Put the file in the best-fit folder under `notes/`, named in lowercase with hyphens.
3. Set `ai_assisted: "Yes"`.
4. Set `status: "Unverified"`. **Never set `Confirmed`**, and never change another note's status to `Confirmed`. Confirmation needs a human reviewer who tested it or checked an authoritative source.
5. Record only what the user told you or what you can cite. Do not invent API parameters, response fields, error messages, version numbers, or behavior. If you aren't sure, write "Not tested" or "Unknown".
6. In `source`, say where the information came from (the user's testing, a meeting date, a documentation URL). In `Verification`, say honestly what was and wasn't tested.
7. Open a pull request from a branch. Never push to `main`.

## Never include

Passwords, API or admin secrets, session tokens (KS), `.env` contents, partner IDs, internal URLs or hostnames, or personal information about people. If the user's material contains any, remove or generalize it and tell them.

## Meeting summaries

Place them in `meetings/YYYY-MM-DD.md`. Strip personal names and institution-specific details. Don't promote claims into `notes/` unless the user asks, and then as `Unverified` with `source` set to the meeting date.
