#journal/monthly 
上月：[[<%moment().subtract(1, 'M').format('YYYY-MM')%>]] || 下月：[[<%moment().add(1, 'M').format('YYYY-MM')%>]]
這季度：[[<%moment().format('YYYY-[Q]Q')%>]]
去年：[[<%moment().subtract(1, 'y').format('YYYY-MM')%>]] 
這月的週：[[<% moment().format('YYYY-[W]ww') %>]] || [[<% moment().add(1, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().add(2, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().add(3, 'w').format('YYYY-[W]ww') %>]] || [[<% moment().add(4, 'w').format('YYYY-[W]ww') %>]]

## Monthly Focus

## Monthly To Do
``` tasks
not done
due after <%moment().startOf('month').subtract(1,'d').format('YYYY-MM-DD')%>
due before <%moment().endOf('month').add(1,'d').format('YYYY-MM-DD')%>
sort by due
sort by tag
hide task count
```
## Habits
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Day", 
row["Meditate"] as "🙏",
row["MP and Review"] as "📝",
row["Kegels"] as "💢",
row["Note making"] as "🗒️",
row["Programming"] as "💻",
row["DJ"] as "🎧",
row["Produce"] as "🎹",
row["Healthy"] as "🥗",
row["Strong"] as "💪",
row["Chinese"] as "🀄",
row["Read"] as "📖",
row["Friend"] as "👥",
row["Money"] as "💵",
row["Clean"] as "🧹"
FROM #journal/daily 
WHERE contains(
file.name, "<%moment().format('YYYY-MM')%>"
)
SORT file.name asc
```
# Review
## Thoughts on this month

^thoughtsOnThisMonth

## Identities Review
What work did you do to your identities this month?
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["SWE days"] as "SWE",
row["Musician days"] as "Musician",
row["Sensemaker days"] as "Sensemaker",
row["Girevik days"] as "Girevik",
row["Chinese days"] as "Chinese"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
### [[Software Engineer]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["SWE review"] as "SWE"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**SWE Month Review**:: <br>- 

### [[Musician]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["Musician review"] as "Musician"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Musician Month Review**:: <br>- 

### [[Sensemaker]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["Sensemaker review"] as "Sensemaker"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Sensemaker Month Review**:: <br>- 

### [[Girevik]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["Girevik review"] as "Girevik"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**SWE Month Review**:: <br>- 

### [[Chinese Speaker]]
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week",
row["Chinese review"] as "Chinese"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
**Chinese Month Review**:: <br>- 


## Weekly Reviews

```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Memorable"] as "Memorable"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Takeaways"] as "Takeaways"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```

```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Start"] as "Start",
row["Continue"] as "Continue",
row["Stop"] as "Stop"
WHERE (
file.name = "<% moment().format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```

## Media
```dataview
TABLE WITHOUT ID link(file.link, default(file.aliases[0], file.name)) AS "Week", 
row["Music"] as "Music",
row["Podcasts"] as "Podcasts",
row["TV"] as "TV",
row["Movies"] as "Movies",
row["Books"] as "Books"
WHERE (
	file.name = "<% moment().format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
	file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```



## Toggl
```toggl
SUMMARY FROM <%moment().startOf('month').format('YYYY-MM-DD')%> TO <%moment().endOf('month').format('YYYY-MM-DD')%>
SORT DESC
```


