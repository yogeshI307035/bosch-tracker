# Bosch Sales Cloud Impediment Tracker

Public mirror of the Bosch v2+FSM impediment tracker, auto-refreshed from SharePoint daily.

🔗 **Live site:** https://yogeshi307035.github.io/bosch-tracker/

## How it works

- `index.html` — kanban UI (static, self-contained)
- `data/data.json` — parsed impediment data from the Bosch SharePoint workbook
- Local Mac launchd job runs daily at 08:15, refreshes the data, and pushes to this repo.
- Your personal notes live in `localStorage` in your browser — they don't sync here.

## Local dev

The authoring copy of this tracker lives at `~/pm-dashboard/bosch-tracker/` on the author's Mac.
The local version has a Refresh button that triggers the full SharePoint → parse → publish pipeline.
This public version has a Reload button that just re-fetches the latest `data/data.json` from the site.
