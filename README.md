# json-surgery

Reliable JSON transformation for AI-augmented software.

`json-surgery` helps you apply natural-language changes to JSON safely and predictably. Instead of asking a model to rewrite an entire document in one shot, it breaks the work into small atomic operations, verifies each step, and iterates until the result matches your intent.

This is built for teams that want access to the power and flexibility of AI, without giving up control.

## Why teams use it

- Reduce breakage from one-shot JSON rewrites.
- Keep large, nested, or irregular payloads stable during edits.
- Add validation gates so business rules are enforced before output is accepted.
- Keep visibility into in-progress transformations during long or complex edits.
- Recover gracefully when limits are hit, with access to the last known state.

## What problems it solves

- Normalizing external-source data from clients, vendors, partners, or user-uploaded payloads.
- Cleaning and restructuring semi-structured JSON during ingestion.
- Applying policy-driven changes across many nested records.
- Powering agent workflows that need deterministic JSON changes, not approximate rewrites.

## How it works

1. You provide a JSON object and plain-language modification instructions.
2. `json-surgery` converts the request into discrete operations such as assign, delete, append, insert, and rename.
3. Operations are validated and applied iteratively, with optional feedback loops between rounds.
4. You receive a transformed object that reflects the requested changes with far higher reliability than direct full-document generation.

## What makes it different

- Edit-based, not rewrite-based: safer for complex objects.
- Designed for production guardrails: validation, progress hooks, and bounded execution.
- Practical for real-world messy data: especially external payload normalization.
- Maintained as a cross-runtime project with aligned behavior.

## Who this is for

- AI product teams shipping structured-data features.
- Platform and backend teams maintaining strict JSON contracts.
- Data and automation teams standardizing incoming payloads before downstream processing.

## Explore Package Docs

- [packages/python-json-surgery/README.md](packages/python-json-surgery/README.md)
- [packages/typescript-json-surgery/README.md](packages/typescript-json-surgery/README.md)
