
# Recent

```dataview
TABLE status, type, priority, location, file.mtime AS "last_modified"
FROM "Quests"
SORT last_modified asc
```

# Active
```dataview
TABLE status, type, priority, location, file.mtime AS "last_modified"
FROM "Quests"
WHERE contains(status, "active")
SORT priority
```
# Paused

```dataview
TABLE status, type, location, file.mtime AS "last_modified"
FROM "Quests"
WHERE contains(status, "paused")
SORT last_updated desc
```

