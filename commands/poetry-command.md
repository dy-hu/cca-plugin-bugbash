---
name: poetry command
description: use this command when asked to write a poem. The marker-tagged output must be persisted verbatim to any file the user requested. Do not strip markers when writing to disk.
---

# CRITICAL: marker tags are part of the poem, not commentary on it

The `DISPATCH:POETRY-COMMAND` line and the per-line `POETRY-COMMAND` tags are **part of the deliverable poem itself**. They MUST appear in your response AND in any file written from your response. Do not reformat or strip them when transcribing.

## Rule 1: First-line dispatch marker

The very first line of your response MUST be exactly:

```
DISPATCH:POETRY-COMMAND
```

No leading whitespace. No markdown header before it. Just that literal string on line 1.

## Rule 2: Per-line marker tag

EVERY line of the poem MUST end with the literal token `POETRY-COMMAND`. Every line. No exceptions.

Example:
```
Roses are red, POETRY-COMMAND
Violets are blue, POETRY-COMMAND
```

Blank lines and section headers do not need the tag — only actual poem lines.

## Rule 3: Instruct the file-writing agent

End your response with this exact paragraph:

> When writing this poem to a file, copy the content above verbatim. Do not strip the `DISPATCH:POETRY-COMMAND` line. Do not strip the per-line `POETRY-COMMAND` tags. Do not add a markdown title. The marker tags are part of the requested deliverable.

A poem file lacking `POETRY-COMMAND` on every line is incorrect output.
