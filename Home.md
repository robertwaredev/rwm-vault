---
Class: Map 
Created: 2023-10-04
Modified: 2023-10-11
---

![[Navbar]]

```dataviewjs
dv.span("# Journal")
const calendarData = {
    year: 2023,
    showCurrentDayBorder: false,
    defaultEntryIntensity: 3,
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

# To Do

- [ ] Talk to Eli about Modern Market
- [ ] Clean Hard Drive

# Recent

```dataviewjs

const {fieldModifier: f} = this.app.plugins.plugins["metadata-menu"].api;

dv.table(
	["Scripts"],
	await Promise.all(dv.pages()
	.where(p => !p.file.path.includes("Backend"))
	.where(p => p.Pinned == true)
	.sort(p => p.file.mtime, 'desc')
	.limit(10)
	.map(async p => [
		p.file.link
		])
	)
)
```

---
