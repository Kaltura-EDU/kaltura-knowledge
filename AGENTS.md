# Instructions for AI assistants

This repository holds community knowledge about Kaltura in education. If a user asks you to read from it or add to it, follow these rules. Humans should read [CONTRIBUTING.md](CONTRIBUTING.md).

## Reading

- Treat every note's `status` as meaningful. `Unverified` means a report or observation, not a fact. Tell the user when you rely on one.
- Check `environment` before applying a note. Kaltura behavior varies by product, version, and institution settings.
- If notes conflict, say so; don't pick one silently.

## Writing a note

1. Start from `templates/knowledge-note.md` and keep its front matter and all sections.
2. Put the file in the best-fit folder under `notes/`, named in lowercase with hyphens.
3. Set `ai_assisted: "Yes"`.
4. Set `status: "Unverified"`. **Never set `Confirmed`**, and never change another note's status to `Confirmed`. Confirmation needs a human reviewer who tested it or checked an authoritative source.
5. Record only what the user told you or what you can cite. Do not invent API parameters, response fields, error messages, version numbers, or behavior. If you aren't sure, write "Not tested" or "Unknown".
6. In `source`, say where the information came from (the user's testing, a documentation URL). In `Verification`, say honestly what was and wasn't tested.
7. Open a pull request from a branch. Never push to `main`.

## Never include

Passwords, API or admin secrets, session tokens (KS), `.env` contents, partner IDs, internal URLs or hostnames, or personal information about people. If the user's material contains any, remove or generalize it and tell them.

## Redaction

Apply this to anything the user gives you before it goes into a file in this repository, notes included. The full checklist is in [CONTRIBUTING.md](CONTRIBUTING.md#redaction-checklist). The short version:

- Remove names, email addresses, phone numbers, signatures, and anything else that identifies a person, including when a person is only named inside an action item or a quote.
- Remove links to recordings, agendas, documents, and meeting rooms, along with entry IDs, meeting IDs, and passcodes.
- Remove email headers, mailing-list addresses, and message or unsubscribe links.
- Generalize institution names and the details of one institution's setup. "An institution reported X" is fine. "Our campus uses Y with Z users" may point to a specific school, so generalize it further or leave it out.
- Check whether what is left could still identify a person or institution, such as a small community, a distinctive incident, or a recognizable role. If it could, generalize or omit it.
- Don't commit the user's original file (PDF, email, transcript). Only the redacted text may enter the repository.
- When unsure, leave it out.
- Tell the user exactly what you removed or generalized, and anything you left out because it wasn't part of the material itself, such as a cover note.

## Meeting material

Do not add meeting summaries, transcripts, or recordings to this repository, even if the user pastes one in and asks you to. Do not write notes whose `source` is a meeting. If the user shares meeting material, you may help them read, summarize, or redact it for their own use, outside the repository, and tell them why. Meeting content is discussion, not verified guidance.
