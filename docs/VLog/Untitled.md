```dataview
TABLE status, file.ext AS type
     WHERE contains(lower(file.name), "obsidian")
    SORT status ASC
```
