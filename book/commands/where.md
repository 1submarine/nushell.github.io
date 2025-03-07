---
title: where
version: 0.67.0
usage: |
  Filter values based on a condition.
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> where (cond) --block```

## Parameters

 -  `cond`: condition
 -  `--block {block}`: use where with a block or variable instead

## Examples

List all files in the current directory with sizes greater than 2kb
```shell
> ls | where size > 2kb
```

List only the files in the current directory
```shell
> ls | where type == file
```

List all files with names that contain "Car"
```shell
> ls | where name =~ "Car"
```

List all files that were modified in the last two weeks
```shell
> ls | where modified >= (date now) - 2wk
```

Get all numbers above 3 with an existing block condition
```shell
> let a = {$in > 3}; [1, 2, 5, 6] | where -b $a
```
