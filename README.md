# Evergreen Planner

Responsive school and productivity planner. Open `index.html` in a current browser; it has no build step or package installation.

Features include dashboard, tasks, homework, calendar day/week/month/year views, weekly timetable, projects, study-session suggestions, focus timer, statistics, theme settings, reminders, and JSON backup/restore. Study suggestions use the configured study days and hours, session size, daily limit, homework deadline, and timed calendar events. The app reports when estimated minutes do not fit.

Planner data is stored in this browser on this device. It does not sync to the cloud or across devices. Export backups in Settings. Do not enter sensitive personal data.

Google Calendar, Outlook, and Apple Calendar are listed in the Connections area but are not yet live integrations. Real calendar sync needs a secure backend for OAuth/CalDAV and token storage; do not place provider secrets or Apple credentials in static browser code. Sparx Maths and Educake are manual entry because no authorized official API is configured. This app does not scrape those sites or bypass their access controls.

## GitHub Pages

Upload the contents of this folder to the root of a repository. In repository Settings → Pages, choose **Deploy from a branch**, `main`, and `/(root)`. The site is static and needs no build step.

Cloud accounts and multi-device persistence require a server-backed edition with Supabase Auth and Row Level Security. Never expose service keys or Microsoft secrets in browser code.
