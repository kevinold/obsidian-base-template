<% tp.file.include('[[Frontmatter (Template)]]') %>

# [[<% tp.file.title %>]]


## 📋 Tasks

- [ ] Review calendar for the week
- [ ] Determine what outcomes are relevant for next week
- [ ] Setup meetings for next week


<% tp.file.cursor() %>


<% tp.file.include('[[Projects in the last week (Template)]]') %>


<% tp.file.include('[[Recent Notes (Template)]]') %>


## 🎉 Successes
- 

### ⛰ Obstacles

_What challenges presented themselves this week?_

- 

### 🎒 Lessons Learned

_What would I like to do better next week?_

- 

### 📖 Miscellaneous

- 

## 🗓️ Daily Notes

```dataview
LIST
FROM #type/timeline/daily
WHERE week = <%tp.date.now("ww")%>
```

---

## 📇 Additional Metadata

- 🗂 Type:: #type/timeline/weekly
- 🗓️ Week:: <% tp.date.now("ww") %>