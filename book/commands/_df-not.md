---
title: df-not
version: 0.67.0
usage: |
  Inverts boolean mask
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> df-not ```

## Examples

Inverts boolean mask
```shell
> [true false true] | into df | df-not
```
