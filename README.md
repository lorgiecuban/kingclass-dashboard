# KingClass Academy — Management Dashboard

Live dashboard for internal reporting and monthly performance tracking.

**Live site:** https://lorgiecuban.github.io/kingclass-dashboard/

## Monthly Update Workflow

### Option A — Upload via the UI (session-only)
1. Open the live URL
2. Go to the **Upload Data** tab
3. Upload the Curriculum CSV and/or Grade CSV for the new month
4. Data is available for that browser session

### Option B — Bake the new month into the file (persists for everyone)
1. Export the month's data as CSV
2. Edit `index.html` — find `RAW_CURR` and `RAW_GRADE` near the top of the `<script>` block
3. Append new rows in the compact format: `{m:"March",y:2026,bc:"N001",bn:"เชียงราย",c:"KingMath",s:150,r:225000}`
4. Commit and push — the live page updates within minutes

## CSV Format Reference

**Curriculum CSV**
```
Month,Year,Branch Code,Branch Name,Curriculum,Students,Revenue
March,2026,N001,เชียงราย,KingMath,150,225000
```

**Grade CSV**
```
Month,Year,Branch Code,Branch Name,Grade,Students,Revenue
March,2026,N001,เชียงราย,ป.1,25,37500
```
