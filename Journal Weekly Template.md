#journal/weekly 
上週：[[<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>]] || 下週：[[<% moment().add(1, 'w').format('YYYY-[W]ww') %>]]
這個月：[[<% moment().format("YYYY-MM") %>]]
去年：[[<% moment().subtract(1, 'y').add(1, 'w').format('YYYY-[W]ww') %>]]

[[<% tp.date.weekday("YYYY-MM-DD", 0) %>]] || [[<% tp.date.weekday("YYYY-MM-DD", 1) %>]] || [[<% tp.date.weekday("YYYY-MM-DD", 2) %>]] || [[<% tp.date.weekday("YYYY-MM-DD", 3) %>]] || [[<% tp.date.weekday("YYYY-MM-DD", 4) %>]] || [[<% tp.date.weekday("YYYY-MM-DD", 5) %>]] || [[<% tp.date.weekday("YYYY-MM-DD", 6) %>]]



# Planning
## Intention setting
Priorities:: <br>- 
Possible obstacles::<br>- 
Events::<br>- 
## Calendar
- [ ] Review your [calendar](https://calendar.google.com) last week. 

- Did you follow it? Did you get distracted?
- Improvements?

- [ ] Plan this week in your [calendar](https://calendar.google.com) 📅 <%moment().startOf('week').format('YYYY-MM-DD')%>

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
WHERE (
file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>"
)
SORT file.name asc
```

## Weekly To do
- [ ] Review [[accomplishments]]
- [ ] Review [[regrets]]
- [ ] Review this week 📅 <%moment().endOf('week').format('YYYY-MM-DD')%>
- [ ] Review month 
- [ ] Review quarter 
- [ ] Review [[My Values]] [[My identities]] 
- [ ] Call mom 
- [ ] call miles 
- [ ] Call marianna 

# Reviews
[[Questions]]

## Identities Review
- [ ] What work did you do to your identities this week?
### [[Software Engineer]]
**SWE days**:: /7
**SWE review**::<br>- 

### [[Musician]]
**Musician days**:: /7
**Musician review**::<br>- 

### [[Sensemaker]]
**Sensemaker days**:: /7
**Sensemaker review**::<br>-

### [[Girevik]]
**Girevik days**:: /7
**Girevik review**::<br>- 

### [[Chinese Speaker]]
**Chinese days**:: /7
**Chinese review**::<br>- 

## Task Review
- [ ] Are you doing the things you're supposed to? If not, what are the things getting in your way?

## Experiment Review
- [ ] If you're running an experiment, how is it going?

## Toggl review
- [ ] review [Toggl](http://track.toggl.com). 
Are you happy with how you spent your time?

## Media
**Music**:: 
**Podcasts**:: 
**TV**:: 
**Movies**:: 
**Documentaries**:: 
**Books**:: 

## Summaries
[[<% tp.date.weekday("YYYY-MM-DD", 0) %>#^quickSummary]] 
[[<% tp.date.weekday("YYYY-MM-DD", 1) %>#^quickSummary]] 
[[<% tp.date.weekday("YYYY-MM-DD", 2) %>#^quickSummary]] 
[[<% tp.date.weekday("YYYY-MM-DD", 3) %>#^quickSummary]] 
[[<% tp.date.weekday("YYYY-MM-DD", 4) %>#^quickSummary]] 
[[<% tp.date.weekday("YYYY-MM-DD", 5) %>#^quickSummary]] 
[[<% tp.date.weekday("YYYY-MM-DD", 6) %>#^quickSummary]]




## Mood and Health
```dataview
table 
row["AM Mood"] as "🌇",
row["PM Mood"] as "🌆",
row["Workout"] as "🏋️‍♂️",
row["Mobility"] as "🧘‍♂️",
row["Steady state"] as "🏃‍♂️"
FROM #journal/daily 
WHERE (file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>")
SORT file.name asc
```
## Food
```dataview
table 
row["Calories"] as "Calories",
row["Weight"] as "Weight"
FROM #journal/daily 
WHERE (file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>")
SORT file.name asc
```
## Five Minute Journal
```dataview
table 
row["I am grateful for"] as Gratitude, 
row["What went well"] as "What went well?", 
row["What could have gone better"] as "Could go better?", 
row["Notable things"] as "Notable things"
FROM #journal/daily 
WHERE (
file.name = "<% tp.date.weekday("YYYY-MM-DD", 0) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 1) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 2) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 3) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 4) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 5) %>" or
file.name = "<% tp.date.weekday("YYYY-MM-DD", 6) %>"
)
SORT file.name asc
```

### Toggl weekly summary
```toggl
SUMMARY FROM <% tp.date.weekday("YYYY-MM-DD", 0) %> TO <% tp.date.weekday("YYYY-MM-DD", 6) %>
SORT DESC
```
## Weekly Review
- What were my priorities this week? How did they go?
- What got neglected this week? Why did that happen?
- What were some wins this week? What made them great?

**Start**::<br>- 
**Continue**::<br>- 
**Stop**::<br>- 
**Takeaways**:: <br>- 
**Memorable**::<br>- 

