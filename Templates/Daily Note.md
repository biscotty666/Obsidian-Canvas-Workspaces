%%
type:: template
dates:: {{date}}
tags:: #log/journal #note/daily 
%%
## <% tp.file.title %>

### Quote

<% tp.web.daily_quote() %>

### Reflections
#### Thoughts
#### Progress

### Tasks

#### New today


```todoist
name: ""
filter: "created: <% tp.date.now("MMM Do YYYY") %>"
```



#### Due today

```todoist
name: "Due Today"
filter: "<% tp.date.now("MMM Do YYYY") %>"
sorting: 
  - date
  - priority
group: true
```

#### Priority 1 tasks

```todoist
name: ""
filter: p1
```

#### Undated Tasks
```todoist
name: ""
filter: no date
group: true
```

### Logs
#### Exercise Log
```dataview
table without id
type as Type, time as Time, distance as Distance, route as Route, notes as Note, image as Photo
from #log/exercise 
where date = date("<% tp.date.now("YYYY-MM-DD") %>")
```
#### Study Log
```dataview
table without id
topic as Topic, file.name as Reference, note as Note, date as Date, related as Related, references as References
from #log/study & -"Extras/Templates"
where date = date("<% tp.date.now("YYYY-MM-DD") %>")
```

#### Project

```dataview
table without id
topic as Topic, file.name as Reference, note as Note, related as Related, references as References
from #log/project & -"Extras/Templates"
where date = date("<% tp.date.now("YYYY-MM-DD") %>")
```

#### Infrastructure
```dataview
table without id
topic as Topic, file.name as Reference, notes as Notes, inf-related as Related, references as References
from #log/infrastructure  & -"Extras/Templates"
where date = date("<% tp.date.now("YYYY-MM-DD") %>")
```


#### Piano Log
```dataview
table without id
topic as Topic, file.name as Reference, notes as Notes, inf-related as Related, references as References
from #log/piano  & -"Extras/Templates"
where date = date("<% tp.date.now("YYYY-MM-DD") %>")
```

#### Domestic Log
```dataview
table without id
topic as Topic, file.name as Reference, notes as Notes, inf-related as Related, references as References
from #log/domestic  & -"Extras/Templates"
where date = date("<% tp.date.now("YYYY-MM-DD") %>")
```

---
### Yesterday's Note

<%*
const yesterday = tp.date.yesterday("YYYY-MM-DD")
tR += "![[" + [[yesterday]] + "]]"
%>


