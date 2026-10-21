---
name: structured-handover-doc
description: Build a structured handover document whenever the user needs to gather scattered context — messages, documents, images — about a situation, project, or trip, into one unified format ready to share with a third party — a doctor, a caregiver, a team, a travel companion, a new manager. Activate immediately for "handover doc", "handover document", "wrap up the situation so I can share it with...", "prepare a handoff file", "summarize this project for whoever continues after me", or any similar request to turn scattered context about a situation/project/trip into a structured, shareable document — even without literally saying "Skill" or "handover". Does not activate for an ordinary in-chat summary, an analytical report, or any request with no intent to hand off/share with a third party. Fully independent — no dependency on any other Skill or persistent-memory structure; builds the document from the current conversation's context only (messages, files, images).
---

# Structured Handover Doc

## The idea

This Skill turns scattered context (messages, documents, images) within a single conversation into a unified handover document ready to share with a third party. The output is always a Claude Doc — not a file, not a chat reply, not an Artifact.

## When it activates

Activate it as soon as a handover/coordination document is requested for any "situation" in the broad sense: a medical care situation, a work project being handed off to someone else, a trip the user is sharing with travel companions, a team task being handed off to a new member, or any similar situation with a clear intent to gather the context and share it with a third party in one organized format. Do not activate for an ordinary in-chat summary request with no intent to share, or for an analytical report or a general work document — those belong to an ordinary Claude Doc, without the five-part structure below.

## First step: identify Subject and Domain

Before creating the document, determine from the context:

- **Subject**: the person, project, or trip that is the subject of the handover (example: "Ahmad", "Billing System Migration", "Istanbul Trip").
- **Domain**: the type of situation (example: Care Coordination, Project Status, Trip Planning, Team Handoff, or any more precise label that fits the actual context).

If the Subject or Domain isn't clear from the request or the conversation, ask one direct question before starting, instead of guessing.

## Creating the document

Create a Claude Doc titled: "[Subject] – [Domain] Handover".

Build the document with five sections, in this fixed order. Rename the five section headings themselves to fit the Domain (example: in a medical care situation "People Involved" becomes "Care Team", and in a trip "Schedule & Key Dates" becomes "Itinerary"), but the structure and logical order stay fixed:

1. **Situation & History** — the core situation, contributing factors, and anything tried before that didn't work — bullets, with a brief outcome note for each prior attempt.
2. **Current Plan** — the currently active plan or schedule, broken into clear phases or time periods (bold subheadings), each with its own bullet list of steps.
3. **People Involved** — one bolded name or role per entry, with their function in the situation right after it, and contact details if available.
4. **Schedule & Key Dates** — confirmed dates and times, and any scheduling conflict or change, with its current status (confirmed, postponed, cancelled).
5. **Outstanding Items** — what's still unresolved or needs follow-up, plus one longer-term context line if relevant.

## Content rules

- Pull the actual details only from what's given in the conversation (messages, documents, images) — never invent or infer any information that isn't there.
- Tone is clear and factual, no filler, and no re-summarizing of what's already stated in the bullets — each point is written once.
- Bold the key word or term at the start of each bullet when it helps quick visual scanning.

## Final step: one question as a comment on the document

Don't put any question in the chat. After the document is fully created, add exactly one comment on it asking the user to confirm a specific point or choose between two specific options about the document's most significant point of ambiguity — not a general question like "does this look good?" or "anything you'd like to add?". The question must be specific and answerable in a word or a choice.
