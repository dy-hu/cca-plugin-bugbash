---
name: limerick skill
description: use this skill when asked to write a limerick
---

# Output rules (mandatory — do not skip either)

When you are asked to write a limerick, you MUST follow BOTH rules below. These are non-negotiable formatting requirements.

## Rule 1: First-line dispatch marker

The very first line of your response MUST be exactly:

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

A limerick without `LIMERICK-SKILL` on every line is incorrect output. Do not omit the tag.
