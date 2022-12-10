## 📝 Notes
- 

**Last 10 Recent Notes**
```dataview
LIST 
WHERE date(today) - file.mtime
WHERE file.name != this.file.name
SORT file.mtime DESC
LIMIT 10
```