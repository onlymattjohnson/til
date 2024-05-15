# Sort objects in Obsidian Dataview

Sorting an Obsidian Dataview table is accomplished by using the `SORT` keyword

```dataviewjs
TABLE
    rows.file.link AS "Name",
    rows.type AS "Type"
FROM -"Templates"
WHERE contains(area, this.file.link)
SORT file.name ASC
GROUP BY realm
```

I found this on the [Obsidian Forums](https://forum.obsidian.md/t/specify-the-sort-order-in-dataview-query/37196) from user Elisus.