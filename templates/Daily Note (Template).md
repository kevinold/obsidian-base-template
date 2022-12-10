<% tp.file.include('[[Frontmatter (Template)]]') %>

# [[<% tp.file.title %>]]


## 📋 Tasks

- [ ] Review calendar today
- [ ] Finalize Notes and Learnings
- [ ] Determine what outcomes are relevant for today
- [ ] Setup / reschedule meetings

## 💼 Meetings
- [[<% tp.date.now("YYYYMMDD") %> - ]]
- <% tp.file.cursor() %>

```dataview
LIST
WHERE contains(file.name, "<% tp.date.now("YYYYMMDD") %>")
```

## 🛤 Tracking

**List of Notes in Last 3 days**
```dataview
LIST WHERE date(today) - file.mtime <= dur(3 days)
WHERE file.name != this.file.name
SORT file.mtime DESC
LIMIT 10
```

### Customer issue(s)
- 

<% tp.file.include('[[Projects in the last week (Template)]]') %>

<% tp.file.include('[[Recent Notes (Template)]]') %>


### ❓Questions
- 


### 💡Ideas
- 

### 👀 Observations

- 

### ⛰ Obstacles

_What challenges presented themselves?_

- 

### 🎒 Lessons Learned

_What would I like to do better tomorrow?_

- 

### 📖 Miscellaneous

- 

## 📆 Follow up

 - 

---

## 📇 Additional Metadata

- 🗂 Type:: #type/timeline/daily 
- 🗓️ Week:: <% tp.date.now("ww") %>