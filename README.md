# Evergreen Planner

Evergreen Planner is a student productivity planner with a dashboard, tasks, homework, calendar, weekly timetable, projects, study-session suggestions, focus timer, statistics, theme settings, reminders, and JSON backup/restore.

## Download the desktop app

Desktop packages are built for Windows, macOS, and Linux using Electron.

- **Windows installer:** download the setup EXE from the [latest desktop release](https://github.com/nhktop/evergreen-planner/releases/tag/desktop-latest), then run it.
- **Windows portable:** download the portable EXE from the same release; it can run without installation.
- **macOS / Linux:** download the matching DMG or AppImage from the workflow artifacts.

The GitHub Actions workflow rebuilds the desktop packages whenever changes are pushed to main. Windows installers are published to the latest desktop release. Build artifacts for all three platforms are available in the workflow run for 30 days.

## Run from source

Requires Node.js 22 or later.

```bash
npm install
npm start
```

## Local data and integrations

Planner data is stored in the app's local browser storage on this device. It does not currently sync to the cloud or across devices. Export backups in Settings. Do not enter sensitive personal data.

Google Calendar, Outlook, and Apple Calendar are listed in Connections but are not yet live integrations. Real calendar sync needs a secure backend for OAuth/CalDAV and token storage; do not place provider secrets in desktop frontend code. Sparx Maths and Educake are manual entry because no authorized official API is configured. This app does not scrape those sites or bypass their access controls.

## GitHub Pages

The same files continue to power the browser version: https://nhktop.github.io/evergreen-planner/