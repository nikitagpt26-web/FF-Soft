# CLAUDE.md — FF-Soft

## Important: public repository; private operational data

This is the intended **FF Москва warehouse inventory interface** codebase. The repository was empty when inspected on 2026-10-19. Do not infer that any application, database, WMS integration, or stock accounting is already implemented.

**This repository is PUBLIC.** Never commit client names, private quotes/rates, shipping details, internal barcodes/KIZ, actual quantities, sales reports, credentials, screenshots from production systems or other private warehouse/customer information.

The canonical internal product handoff is in the **separate private repository** `nikitagpt26-web/-web-studio-lab`:

- `archive/ai-bridge/FF_SOFT_HANDOFF_2026-10-19.md`
- `archive/ai-bridge/CLAUDE_GPT_WORKFLOW_2026-10-19.md`
- `archive/ff-moscow/README.md` and its linked historical operational files
- `USER_CONTEXT.md` (cross-project founder preferences)

Read these **only with legitimate authenticated access**. Do not copy them into the public repo, public logs or third-party model requests. If access is unavailable, say so instead of guessing.

## Broad technical product direction (non-sensitive)

Build a fast, reliable multi-client inventory interface for receiving, SKU/barcode lookup, addressed storage, container relocation, reservations, pick/dispatch, returns, cycle counts and auditable stock movements. V1 should prioritize error prevention and minimal picker interactions over an oversized management dashboard. Avoid inventing live WMS integrations or data mappings.

Critical engineering properties: strict tenant scoping, atomic/idempotent movements, recoverable scan/print failures, stock conservation and traceability, safe concurrent allocations, human-approved imports and marketplace write operations. Use synthetic demo data in this public repository.

## Claude / GPT handoff

Claude Code should use this local file as project entrypoint, follow the private handoff if available, and work in small tested GitHub commits. GPT/Codex review is optional and only considered performed if a working authenticated tool or actual persisted review exists. Project files do not themselves install a cross-model connector.

## First implementation task

Inspect the repository state, confirm scope with the founder if required, then create a narrow V1 plan and build the smallest working synthetic-data flow. Do not claim production readiness or import real records without authorization.
