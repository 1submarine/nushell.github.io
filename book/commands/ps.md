---
title: ps
version: 0.67.0
usage: |
  View information about system processes.
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> ps --long```

## Parameters

 -  `--long`: list all available columns for each entry

## Examples

List the system processes
```shell
> ps
```

List the top 5 system processes with the highest memory usage
```shell
> ps | sort-by mem | last 5
```

List the top 3 system processes with the highest CPU usage
```shell
> ps | sort-by cpu | last 3
```

List the system processes with 'nu' in their names
```shell
> ps | where name =~ 'nu'
```
