---
related:
  - '[[<% tp.date.now("YYYY") %>]]'
---
## Weekly Notes


```dataview
LIST FROM "journals" AND -"journals/weekly"
WHERE contains(related, [[<% tp.date.now("YYYY") %>-W<% tp.date.now("ww") %>]])
SORT file.name ASC
```