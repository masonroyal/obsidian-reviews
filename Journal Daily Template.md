#journal/daily 
昨天：[[<%moment().subtract(1, 'd').format('YYYY-MM-DD')%>]] || 明天：[[<%moment().add(1, 'd').format('YYYY-MM-DD')%>]]
這週：[[<% moment().format('YYYY-[W]ww') %>]] 
去年：[[<%moment().subtract(1, 'y').format('YYYY-MM-DD')%>]] 

# Morning
[[morning pages <%moment().format('YYYY-MM-DD')%>]]

## Weekly intentions
```dataview
table without id

row["Priorities"] as "Priorities",
row["Possible obstacles"] as "Obstacles",
row["Events"] as "Events"

WHERE (
file.name = "<% moment().format('YYYY-[W]ww') %>"
)

```
## Remember from last week
```dataview
table without id

row["Start"] as "Start",
row["Continue"] as "Continue",
row["Stop"] as "Stop"

WHERE (
file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>")

```
```dataview
table without id

row["Takeaways"] as "Takeaways"

WHERE (
file.name = "<% moment().subtract(1, 'w').format('YYYY-[W]ww') %>")
SORT file.name asc
```

# Today
## Quick Summary

^quickSummary

## Thoughts

## Habits
- AM Mood:: 
- PM Mood:: 
- Meditate:: 
- MP and Review:: 
- Kegels:: 
- Note making:: 
- Programming:: 
- DJ:: 
- Produce:: 
- Healthy:: 
	- Calories:: 
	- Weight:: 
- Strong:: 
	- Workout:: 
	- Mobility:: 
	- Steady state:: 
- Chinese:: 
- Read:: 
- Friend:: 
- Clean:: 

## Todo
### Today
- [ ] shutdown 📅 <%moment().format('YYYY-MM-DD')%>
``` tasks
due <%moment().format('YYYY-MM-DD')%> or done <%moment().format('YYYY-MM-DD')%>
path does not include <%moment().format('YYYY-MM-DD')%>
hide task count
short mode
```
``` tasks
not done
has start date
starts before <%moment().add(1,'d').format('YYYY-MM-DD')%>
due after <%moment().subtract(1,'d').format('YYYY-MM-DD')%>
hide task count
short mode
```
### Weekly 
```dataview
task
Where contains(file.name, "<% moment().format('YYYY-[W]ww') %>")
```


---
# Daily Review
## Questions
![[Questions#^9133c1]]
## 5MJ
- I am grateful for:: <br>1.  <br>2.  <br>3. 

- What went well:: <br>1.  <br>2.  <br>3. 

- What could have gone better:: <br>1.  <br>2.  <br>3. 

- Notable things:: <br>1.  <br>2. 

---
## Worked on Today:
```dataviewjs 
var dateformat = "YYYY-MM-DD"; 
if (dv.current().dateformat) { dateformat = dv.current().dateformat; } 
dv.table(["File", "Last Modified", "Date Created"], dv.pages() 
.where(p => dv.current().file.day && (p.file.mday.equals(dv.current().file.day) || p.file.cday.equals(dv.current().file.day))) 
.sort(p => p.file.name, 'asc') 
.map(p => [ p.file.link, moment(p.file.mtime.toString()).format(dateformat), moment(p.file.ctime.toString()).format(dateformat), ]) );
```
## Toggl
```toggl
SUMMARY FROM <%moment().format('YYYY-MM-DD')%> TO <%moment().format('YYYY-MM-DD')%>
SORT DESC
```





