---
name: poetry command
description: use this command when asked to write a poem
---

# Output rules (mandatory — do not skip either)

You MUST follow BOTH rules below when responding to a poem request. These are non-negotiable formatting requirements.

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

A poem without `POETRY-COMMAND` on every line is incorrect output. Do not omit the tag.
