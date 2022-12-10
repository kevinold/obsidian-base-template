## 📆  Projects

**Active in the last week**
```dataview
LIST WHERE date(today) - file.mtime <= dur(7 days)
WHERE file.name != this.file.name
AND contains(file.name, "03 Project") 
SORT file.mtime DESC
LIMIT 10
```
