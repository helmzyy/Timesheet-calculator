# Time & Pay Calculator

A fast, browser‑only calculator that totals hours, handles overtime, and estimates gross and net pay. Stores history locally with per‑week date ranges and lets you delete entries.

Live on GitHub Pages (example): `https://<your-username>.github.io/<repo-name>/`

---

## Features
- Paste shifts in natural lines, e.g.  
  `8/27/25 5:00am-9:00pm 30 min lunch`  
  `8/28/25 6:15am-6:30pm no lunch`  
  `9/1/25 Labor Day`
- AM/PM parsing and overnight support.
- Lunch deduction: `30 min lunch`, `1 hr lunch`, or `no lunch`.
- Overtime: first **40h** at base rate, remainder at **1.5×**.
- Adjustable withholdings (sidebar):
  - Hourly rate ($/hr)
  - Federal %, Social Security %, Medicare %
  - Healthcare **$ fixed**
  - Misc Withholding **$ fixed**
- Net pay estimate = `Gross - (percentages × Gross) - fixed$`.
- History with **date range** (first to last workday found).
- Delete individual history rows; Clear all history.
- Copy result; Download CSV.
- Works fully offline once loaded.

---

## How to Use
1. Open the site URL in your browser.
2. Enter your **Hourly Rate** and withholding values (defaults provided).
3. Paste your time entries in the **Paste Hours** box, one per line.
4. Click **Calculate**.
5. Review:
   - Daily cards with net minutes per line
   - Totals (H:MM and decimal hours)
   - Gross and Net (estimated)
6. History section shows saved entry with date range, totals, gross, and net. Use **Delete** to remove an entry or **Clear History** to wipe all.

> Tip: On iPhone, open in Safari → **Share → Add to Home Screen** to make it a one‑tap app.

---

## Deploy to GitHub Pages
1. Put `index.html` and `style.css` in the repo root (add `README.md` if you want).
2. In **Settings → Pages**, set Branch to `main` and Folder to `/ (root)`.
3. Open the provided URL.

---

## Notes
- History is saved to your browser’s `localStorage` on the device where you calculate.
- This app does not transmit data to a server.
- Withholding defaults are simple placeholders; consult a tax pro for your exact situation.

---

## License
MIT
