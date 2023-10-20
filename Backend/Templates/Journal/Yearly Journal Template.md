---
Tags: 
Class: Journal
---

![[Navbar]]

```ad-date
title: <% tp.date.now("YYYY") %>

[[<% tp.date.now("YYYY", "P-1Y") %>|<% tp.date.now("YYYY", "P-1Y") %>]] // [[<% tp.date.now("YYYY", "P1Y") %>|<% tp.date.now("YYYY", "P1Y") %>]]
```

# Heatmaps

```dataviewjs
dv.span("** Journal**")
const calendarData = {
    showCurrentDayBorder: false,
    defaultEntryIntensity: 4,
    entries: [],
}

//DataviewJS loop
for (let page of dv.pages().where(p => p.Class == "Journal")) {
    //dv.span("<br>" + page.file.name) // uncomment for troubleshooting
    calendarData.entries.push({
        date: page.file.name,
        intensity: page.file.size,
        color: "orangeToRed",
    })
}

renderHeatmapCalendar(this.container, calendarData)
```

---

# This Year at a Glance

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P0M", tp.file.title, "YYYY") %>|January]]

![[<% tp.date.now("YYYY-MM", "P0M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P1M", tp.file.title, "YYYY") %>|February]]

![[<% tp.date.now("YYYY-MM", "P1M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P2M", tp.file.title, "YYYY") %>|March]]

![[<% tp.date.now("YYYY-MM", "P2M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P3M", tp.file.title, "YYYY") %>|April]]

![[<% tp.date.now("YYYY-MM", "P3M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P4M", tp.file.title, "YYYY") %>|May]]

![[<% tp.date.now("YYYY-MM", "P4M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P5M", tp.file.title, "YYYY") %>|June]]

![[<% tp.date.now("YYYY-MM", "P5M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P6M", tp.file.title, "YYYY") %>|July]]

![[<% tp.date.now("YYYY-MM", "P6M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P7M", tp.file.title, "YYYY") %>|August]]

![[<% tp.date.now("YYYY-MM", "P7M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P8M", tp.file.title, "YYYY") %>|September]]

![[<% tp.date.now("YYYY-MM", "P8M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P9M", tp.file.title, "YYYY") %>|October]]

![[<% tp.date.now("YYYY-MM", "P9M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P10M", tp.file.title, "YYYY") %>|November]]

![[<% tp.date.now("YYYY-MM", "P10M", tp.file.title, "YYYY") %>#Notes]]
```

```ad-clean
title: [[<% tp.date.now("YYYY-MM", "P11M", tp.file.title, "YYYY") %>|December]]

![[<% tp.date.now("YYYY-MM", "P11M", tp.file.title, "YYYY") %>#Notes]]
```

# Notes

- 

# Captures

