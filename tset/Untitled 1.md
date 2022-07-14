---
cssClasses: cards, cards-cover, cards-2-3
---

```dataview
table without id 
	("![](" + poster + ")") as Poster,
	link(file.link, regexreplace(title, "\s\(\d{4}\)", "") + " " + year) as title,
	"⭐ " + onlineRating as "⭐ MAL",
	type,	
	duration,
	OmarHidan
from #OmarHidan
```