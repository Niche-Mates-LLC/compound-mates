---
description: Remove AI slop and LLM generation fingerprints from branch changes
disable-model-invocation: true
---

Run git diff main (and/or more advanced variants as needed) to identify changes in this branch. Remove code that exhibits stylistic discontinuity with surrounding context and bears hallmarks of LLM generation (exhibits LLM generation fingerprints, e.g., AI slop).

Common manifestations include but are not limited to: redundant or contextually anomalous comments; defensive patterns disproportionate to trust boundaries (e.g., excessive try/catch); type coercion workarounds (e.g., `as any` abuse); verbosity or structure atypical for the file's established conventions.

After completion, report what you changed. Keep it compact — minimum length that conveys the work done, no verbose summaries. Prefer natural prose over tables or bulleted/numbered lists; inline lists are acceptable. Avoid cryptic or overly structured output.
