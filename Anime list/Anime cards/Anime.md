---
cssClasses: cards, cards-cover, cards-2-3, table-max
---

```dataview
table without id 
	("![](" + poster + ")") as Poster,
	link(file.link, regexreplace(title, "\s\(\d{4}\)", "") + " " + year) as title,
	"⭐ " + onlineRating as "⭐ MAL",
	type,	
	episodes,
	join(genres, ", ") as genres,
	duration
from "Media DB"  
where type != "[[Inbox/movie|movie]]"
```

