# Process Plan Dashboard

A single-page dashboard for a process setup & ownership tracker (Excel).

- Click **Upload tracker** or drag an `.xlsx` file onto the page.
- Shows an overview (status counts, progress by process area, items needing attention, milestones, load by owner, KPI health), a filterable action tracker, KPI cards, process/plan cards (entry → main process → exit), a RACI grid, and every other sheet as a table.
- Flags are calculated from **Status** and **Target Date**: Overdue, Due soon (≤ 7 days), Blocked, On track, Done.
- The Excel file is read in the browser only and is never uploaded. The last file opened is remembered on that device (localStorage); **Show sample** clears it.

Run it by opening `index.html` in a browser. No build step. Uses SheetJS from cdnjs.
