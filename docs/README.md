# Mill Rd Upkeep (iPhone app)

A home-screen web app built from `Home_Maintenance_Log.xlsx`: 137 recurring tasks for 1715 Mill Rd plus the "Items to add" list.

## Features
- Overdue / Due soon / Up to date counters, using the spreadsheet's own rules (monthly tasks: due 30 days after last done, warning 1 week ahead; longer tasks: due after months × 30.43 days, warning 1 month ahead). Tasks never logged count as overdue.
- One tap on ✓ logs a task as done today (with Undo). Tap a task to edit its date, frequency, season, cost and notes, and to see its history.
- Filter by season, category and search; group by status, category or frequency.
- "To add" list for future items, with a Schedule button that turns an item into a task.
- Export to CSV, backup and restore (Options menu). Works offline after the first load.

## Put it on your iPhone
1. Host this `docs/` folder over HTTPS. With GitHub Pages: repo **Settings → Pages → Deploy from a branch**, pick the branch and the `/docs` folder.
2. Open the Pages URL in **Safari** on the iPhone.
3. Tap **Share → Add to Home Screen**.

Data is stored on the phone (localStorage). Use **Options → Export backup** now and then.

`tasks.json` is the starting data converted from the spreadsheet. It is only used the first time the app opens, or after **Reset**.
