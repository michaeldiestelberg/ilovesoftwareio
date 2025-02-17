---
title: Read in 2025
date: 2025-02-17
author: Michael Diestelberg
description: A running list of all things I read in 2025
---
This is what I'm reading in 2025.

```dataviewjs
let pages = dv.pages('"04 Archive/Readwise"')
  .where(p => p.date >= dv.date("2025-01-01") && p.date < dv.date("2026-01-01"));

dv.table(["Title", "Author", "Category"], 
  pages.map(p => [p.file.link, p.author, p.category])
);
```