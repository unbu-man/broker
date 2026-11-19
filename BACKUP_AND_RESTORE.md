# GitHub Backup and Restore

This repository is the **new primary location** of the BrokerAI project, migrated from the read-only source `sumdevith/Broker` on 19 November 2026.

## Included
- Main project README.
- Chapters 01–10 covering global crypto + forex brokerage planning, safety, engineering, hiring, first sprint and 90-day schedule.
- `tracker/daily_tasks_snapshot_2026-11-18.csv`: 90 calendar-day task rows plus current checkbox states as archived on 18 November 2026.

## Important limitations
- This migration copies **file contents**. It is **not a Git-history transfer**: the original repository's historical commits remain in the old repository. Preserve the old repo or transfer its Git history separately if that matters.
- The CSV is a snapshot. It does not sync automatically with the Google Sheet, and later checkmarks need another export/commit.
- The original live Google Sheet is separate; the CSV preserves task data, not native styling or dashboard controls.
- The old starter ZIP and any local uncommitted source code are not included in this repository unless specifically added and verified later.
- No production trading engine or licensed brokerage was created; these are project plans and a paper-trading-first roadmap.

## Restore the daily tracker
1. Download `tracker/daily_tasks_snapshot_2026-11-18.csv`.
2. Open or import in Google Sheets.
3. Select the `Done ✓` column (B2:B91 for the CSV header layout), choose **Insert → Checkbox**, and ensure all current FALSE/TRUE values map to unchecked/checked.
4. Add a new sheet called `Dashboard` to compute `=COUNTIF('Daily Tasks'!B2:B91,TRUE)/90`.
5. Continue using an updated Google Sheet and periodically export an updated CSV to GitHub.

## Safety
Keep this public repository free of API secrets, personal data, live account credentials, client records, and regulated market data that cannot be redistributed.
