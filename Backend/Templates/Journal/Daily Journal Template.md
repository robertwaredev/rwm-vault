---
Tags: 
Prev: "[[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]]"
Next: "[[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>]]"
Class: Journal
---

![[Navbar]]

```ad-date
title: <% tp.date.now("dddd, MMMM Do, YYYY", 0, tp.file.title, "YYYY-MM-DD") %>

> [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>|<% tp.date.now("dddd", -1, tp.file.title, "YYYY-MM-DD") %>]] // [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>|<% tp.date.now("dddd", 1, tp.file.title, "YYYY-MM-DD") %>]]

<%* if (tp.date.now() === tp.date.weekday("YYYY-MM-DD", 0, tp.file.title)) { %>
> [[<%* tR += tp.date.now("gggg-[W]ww"); %>|Review <% tp.date.now("[Week ]ww") %>]]
<%* } %>
<%* if (tp.date.now() === moment(tp.file.title).daysInMonth()) { %>
> [[<%* tR += tp.date.now("YYYY-MM"); %>|Review <% tp.date.now("MMMM") %>]]
<%* } %>
```

# Agenda

- [ ] 08:00 Morning Pages
- [ ] 10:00 Inbox Zero

# Morning Pages 

> 

## Affirmations

- 

## Blurts

- 

# Notes

- 
# Captures

