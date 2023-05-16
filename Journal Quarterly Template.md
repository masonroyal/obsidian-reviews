#journal/quarterly 
上季度：[[<%moment().subtract(1, 'Q').format('YYYY-[Q]Q')%>]] || 下季度：[[<%moment().add(1, 'Q').format('YYYY-[Q]Q')%>]]
這季度的月：[[<%moment().format('YYYY-MM')%>]] || [[<%moment().add(1, 'M').format('YYYY-MM')%>]] || [[<%moment().add(2, 'M').format('YYYY-MM')%>]]
今年：[[<%moment().format('YYYY')%>]]
去年：[[<%moment().subtract(1, 'y').format('YYYY-[Q]Q')%>]]

## Quarterly Focus

## Identity Goals this Quarter

## Quarterly To Do

# Review

## Thoughts on the month

[[<%moment().format('YYYY-MM')%>#^thoughtsOnThisMonth]] 
[[<%moment().add(1, 'M').format('YYYY-MM')%>#^thoughtsOnThisMonth]] 
[[<%moment().add(2, 'M').format('YYYY-MM')%>#^thoughtsOnThisMonth]] 

## Weekly Reviews
```dataview
table 
row["Memorable"] as "Memorable"
WHERE (
file.name = "<% moment().format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(5, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(6, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(7, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(8, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(9, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(10, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(11, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(12, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```

```dataview
table 
row["Takeaways"] as "Takeaways"
WHERE (
file.name = "<% moment().format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(5, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(6, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(7, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(8, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(9, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(10, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(11, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(12, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```

```dataview
table 
row["Start"] as "Start",
row["Continue"] as "Continue",
row["Stop"] as "Stop",
row["Takeaways"] as "Takeaways"
WHERE (
file.name = "<% moment().format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(5, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(6, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(7, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(8, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(9, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(10, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(11, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(12, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
```dataview
table 
row["Start"] as "Start",
row["Continue"] as "Continue",
row["Stop"] as "Stop"
WHERE (
file.name = "<% moment().format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(1, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(2, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(3, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(5, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(6, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(7, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(8, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(9, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(10, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(11, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(12, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```
## Media
```dataview
table 
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
file.name = "<% moment().add(4, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(5, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(6, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(7, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(8, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(9, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(10, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(11, 'w').format('YYYY-[W]ww') %>" or
file.name = "<% moment().add(12, 'w').format('YYYY-[W]ww') %>"
)
SORT file.name asc
```

## Identity Goals completed this Quarter
``` tasks
done after <%moment().startOf('quarter').subtract(1, 'd').format('YYYY-MM-DD')%>
done before <%moment().endOf('quarter').add(1, 'd').format('YYYY-MM-DD')%>
tags include #t
hide task count
```

## Habits
```dataview
table 
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
file.name = "<% moment().format('YYYY-MM') %>" or
file.name = "<% moment().add(1, 'M').format('YYYY-MM') %>" or
file.name = "<% moment().add(2, 'M').format('YYYY-MM') %>"
)
SORT file.name asc
```

```toggl
SUMMARY FROM <%moment().startOf('quarter').format('YYYY-MM-DD')%> TO <%moment().endOf('quarter').format('YYYY-MM-DD')%>
SORT DESC
```


