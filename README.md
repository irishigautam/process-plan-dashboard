# Process Plan Dashboard

A single-page dashboard for a process setup & ownership tracker (Excel).

- Click **Upload tracker** or drag an `.xlsx` file onto the page.
- Shows an overview (status counts, progress by process area, items needing attention, milestones, load by owner, KPI health), a filterable action tracker, KPI cards, process/plan cards (entry → main process → exit), a RACI grid, and every other sheet as a table.
- **Recruitment Plan** at `/recruitment`: the recruitment process as presented, with each CTO comment applied to the stage it was written against (current step, CTO comments, revised step), the review mechanism, an action plan on the HR tracker's 30/60/90 milestones, KPIs and optional observations. Includes Copy link and Print / PDF.
- Opens on the original HR tracker (BFL_HR_Plan_and_Tracker_12.xlsx, embedded). Uploading a newer tracker replaces it on that device; **Show original** goes back.
- Flags are calculated from **Status** and **Target Date**: Overdue, Due soon (≤ 7 days), Blocked, On track, Done.
- The Excel file is read in the browser only and is never uploaded. The last file opened is remembered on that device (localStorage).

Run it by opening `index.html` in a browser (the recruitment tab is `#recruitment` locally). No build step. Uses SheetJS from cdnjs. `vercel.json` rewrites `/recruitment` to `index.html`.
