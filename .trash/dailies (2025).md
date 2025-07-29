status: #child 
tags: [[raven]] [[spreadsheet]] [[tracker]] [[daily notes]]

```dataview
TABLE WITHOUT ID
file.link AS dateCreated,
timeEntries AS timeCreated,
DaySummary,
transactionSummary,
transactionHistory,
moods,
meds, habits
FROM "5.8 — database/dailies"
SORT date DESC
WHERE number(transactionHistory)
```