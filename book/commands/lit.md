---
title: lit
version: 0.67.0
usage: |
  Creates a literal expression
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> lit (literal)```

## Parameters

 -  `literal`: literal to construct the expression

## Examples

Created a literal expression and converts it to a nu object
```shell
> lit 2 | into nu
```
