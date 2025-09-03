# Time & Pay Calculator — Pro

A browser‑only time calculator with weekly overtime, net pay estimates, history, JSON import/export, a live clock‑in/out helper, and a clean mobile‑friendly UI with dark mode.

Live via GitHub Pages: `https://<your-username>.github.io/<repo-name>/`

---

## Highlights
- **Weekly grouping & OT**: Uses your chosen start day to group by work week; overtime at **1.5×** after 40h **per week**.
- **Multiple rates**: Optional weekend rate for Sat/Sun lines.
- **Withholdings**: Federal, SS, Medicare (percent), Healthcare & Misc (fixed $/week), plus unlimited **custom deductions** (% or $).
- **Rounding & auto-break**: Round each shift to nearest 5/15 minutes; auto‑deduct a break if shift > 6h.
- **History**: Save each calculation with date range; filter, export CSV, delete rows, or export/import JSON.
- **Clock In/Out**: Timer or manual entry to append cleanly formatted lines.
- **Chart**: Weekly gross vs. net (simple SVG bar chart).
- **Mobile UX**: Sticky button bar; add to Home Screen on iOS.
- **Dark mode**: Toggle persists across reloads.

> All data is local to your browser — no servers involved.

---

## Input Examples
```
8/27/25 5:00am-9:00pm 30 min lunch
8/28/25 6:15am-6:30pm no lunch
9/1/25 Labor Day
```
- Overnight: if end < start, it’s treated as next day.
- Lunch formats: `X min lunch`, `1 hr lunch`, or `no lunch`.

**Note on rates**: Weekend rate affects pay but not the OT threshold (OT is still based on total hours per week).

---

## How to Use
1. Open the site.
2. Expand **Pay, Withholdings & Rules** to set base rate, optional weekend rate, taxes, fixed withholdings, rounding, auto-break, and custom deductions.
3. Paste shifts (or use **Clock In/Out** to append new lines).
4. Click **Calculate**.
5. Review grouped weekly results, totals, gross and net; the overall summary is saved to **History**.
6. Use **Copy Gross/Net** for quick sharing, or export CSV/JSON as needed.

---

## Deploy to GitHub Pages
1. Put `index.html` and `style.css` in the repo root (add `README.md` if you want).
2. In **Settings → Pages**, set Branch to `main` and Folder to `/ (root)`.
3. Open the provided URL.

---

## Limitations
- Holiday handling: lines with “Holiday” (not “Paid”) are treated as 0 time. If you need paid holidays or custom day multipliers, open an issue or extend the code.
- Overtime rules vary by jurisdiction; validate against your payroll policy.

---

## License
MIT
