NANT Events Website (Public Reports + Password-Protected Admin)

PUBLIC
- / (index.html): HOME + dashboard (current event highlighted + all events list)
- /event.html?id=EVENT_ID : event detail view

ADMIN (password protected)
- /admin : Decap (Netlify CMS) editor for creating/editing events and rows.
- Protected via Netlify Identity (invite-only) + Git Gateway.

DEPLOY
1) Put these files into a GitHub repo (main branch).
2) Netlify: New site from Git -> connect repo.
3) Netlify Site settings -> Identity -> Enable.
4) Identity -> Registration -> Invite only.
5) Identity -> Services -> Enable Git Gateway.
6) Identity -> Invite users (admins).
7) Admins edit at /admin, changes publish automatically.

NOTE
- The current event was auto-selected as the latest event date found in Excel.
