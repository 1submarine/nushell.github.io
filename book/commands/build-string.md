---
title: build-string
version: 0.67.0
usage: |
  Create a string from the arguments.
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> build-string ...rest```

## Parameters

 -  `...rest`: list of string

## Examples

Builds a string from letters a b c
```shell
> build-string a b c
```

Builds a string from letters a b c
```shell
> build-string $"(1 + 2)" = one ' ' plus ' ' two
```
