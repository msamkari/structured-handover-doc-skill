structured-handover-doc

A fully independent Claude Skill — builds a structured handover/coordination document (Structured Handover Document) for any situation, project, or trip, from context scattered across a single conversation (messages, documents, images), into one unified format ready to share with a third party.

## Structure

The output is a Claude Doc titled "[Subject] – [Domain] Handover", with five sections in a fixed order (renamed to fit the domain):

1. Situation & History
2. Current Plan
3. People Involved
4. Schedule & Key Dates
5. Outstanding Items

Always ends with one specific comment on the document (never a question in the chat).

## Independence

Does not depend on any other Skill, or on any persistent-memory structure. Builds the document from the current conversation's context only.

## Files

- `SKILL.md` — the Skill's definition.
- `LICENSE` — PolyForm Noncommercial License 1.0.0.
- `releases/v1/structured-handover-doc.skill` — the packaged bundle, ready to upload and activate.

## Report an Issue / Feedback

Found a bug or have a suggestion? Please open a GitHub Issue in this repository: https://github.com/msamkari/structured-handover-doc-skill/issues
