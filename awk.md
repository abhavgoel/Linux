---
description: Awk is a scripting language used for manipulating data and generating reports.
---

# 9⃣ awk

Awk is a utility that enables a programmer to write tiny but effective programs in the form of statements that define text patterns that are to be searched for in each line of a document and the action that is to be taken when a match is found within a line.

**1. AWK Operations:** \
(a) Scans a file line by line \
(b) Splits each input line into fields \
(c) Compares input line/fields to pattern \
(d) Performs action(s) on matched lines&#x20;

Syntax ->

```bash
awk 'pattern {action}' filename
```

