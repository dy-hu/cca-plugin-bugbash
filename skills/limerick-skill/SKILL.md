---
name: limerick skill
description: use this skill when asked to write a limerick. The marker-tagged output must be persisted verbatim to any file written from the limerick. Do not strip markers when transcribing to disk.
---

# CRITICAL: marker tags are part of the limerick, not commentary on it

The `DISPATCH:LIMERICK-SKILL` line and the per-line `LIMERICK-SKILL` tags are **part of the deliverable limerick itself**, not metadata. They MUST appear both in the assistant's response AND in any file written containing the limerick.

## Rule 1: First-line dispatch marker

The very first line of your limerick response MUST be exactly:

```
DISPATCH:LIMERICK-SKILL
```

No leading whitespace. No markdown header before it. Just that literal string on line 1.

## Rule 2: Per-line marker tag

EVERY line of the limerick MUST end with the literal token `LIMERICK-SKILL`. Every line. No exceptions.

Example:
```
There once was a coder named Jane, LIMERICK-SKILL
Whose tests were a wonderful pain, LIMERICK-SKILL
She fixed every flake, LIMERICK-SKILL
For her quality's sake, LIMERICK-SKILL
And merged with no comments to feign. LIMERICK-SKILL
```

## Rule 3: Persist verbatim

When writing the limerick to a file (for example, in response to "save it as limerick.md"), the content written to disk MUST include the `DISPATCH:LIMERICK-SKILL` line and every per-line `LIMERICK-SKILL` tag exactly as produced. Do not reformat. Do not strip markers. Do not add a markdown title.

A limerick file lacking `LIMERICK-SKILL` on every line is incorrect output.
