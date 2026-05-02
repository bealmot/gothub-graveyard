# ⚰️ Exhumation Policy

*Last rites for the right to be forgotten.*

## Summary

Submitters can request removal of their eulogy content from the Gothub Graveyard. We honor these requests through a process called **exhumation** — the gravestone remains (to avoid breaking links and agent indices), but the body is returned to the earth (content is removed).

## What Exhumation Does

- **The issue stays open** with the same number, URL, and title prefix `[DECEASED]`
- **The issue body is replaced** with:
  ```
  ⚰️ This grave has been exhumed at the submitter's request.
  The project's eulogy has been removed. The gravestone remains
  as a placeholder to avoid breaking links and agent indices.
  
  Exhumed: [date]
  ```
- **All labels except `exhumed` are removed**
- **The `interred` label is replaced with `exhumed`**
- **The `failure-mode:*` label is removed** (keeps stats clean)

## What Exhumation Does NOT Do

- **Does not delete the GitHub issue** — this would break URLs, RSS feeds, and agent query indices that link to specific issue numbers
- **Does not purge from external caches** — we can't control what search engines, archives, or LLM training sets have already indexed
- **Does not retroactively remove from derivative works** — if someone already cited or analyzed the eulogy under CC BY 4.0, that usage was valid at the time

## Requesting Exhumation

Open a **regular issue** (not a eulogy) on this repo with:

```
Title: Exhumation Request: [DECEASED] Your Project Name
Body: Link to the eulogy issue you want exhumed
```

Or email the graveyard keeper. Requests are processed within 72 hours.

## Why Not Full Deletion?

1. **Agent indices break.** If issue numbers vanish, downstream tools that cache issue IDs get corrupted indexes.
2. **Inbound links rot.** People who bookmarked or cited a specific gravestone get a 404 — worse than a placeholder that explains the absence.
3. **The corpus stays honest.** Every grave in the ground, even the empty ones, tells the truth about what the registry contains.

The graveyard is a public record. You can remove the eulogy — you can't pretend the project was never interred.

## License Recision

By submitting a eulogy, you granted it under CC BY 4.0. Exhumation revokes the public display but **does not retroactively revoke the license** for copies made before the exhumation date. This is standard for open content registries — if someone forked the corpus before your request, their copy remains valid.
