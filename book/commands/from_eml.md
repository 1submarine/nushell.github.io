---
title: from eml
version: 0.67.0
usage: |
  Parse text as .eml and create table.
---

# <code>{{ $frontmatter.title }}</code>

<div style='white-space: pre-wrap;'>{{ $frontmatter.usage }}</div>

## Signature

```> from eml --preview-body```

## Parameters

 -  `--preview-body {int}`: How many bytes of the body to preview

## Examples

Convert eml structured data into table
```shell
> 'From: test@email.com
Subject: Welcome
To: someone@somewhere.com

Test' | from eml
```

Convert eml structured data into table
```shell
> 'From: test@email.com
Subject: Welcome
To: someone@somewhere.com

Test' | from eml -b 1
```
