---
title: into df
version: 0.67.0
usage: |
  Converts a List, Table or Dictionary into a dataframe
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> into df ```

## Examples

Takes a dictionary and creates a dataframe
```shell
> [[a b];[1 2] [3 4]] | into df
```

Takes a list of tables and creates a dataframe
```shell
> [[1 2 a] [3 4 b] [5 6 c]] | into df
```

Takes a list and creates a dataframe
```shell
> [a b c] | into df
```

Takes a list of booleans and creates a dataframe
```shell
> [true true false] | into df
```
