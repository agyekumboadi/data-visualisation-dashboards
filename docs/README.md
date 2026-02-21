# Tableau Packaged Workbook (.twbx)

This folder contains the Tableau **Packaged Workbook** (`.twbx`) used to build and reproduce the Tableau dashboard exported as:

- `Tableau_KingCrab_Population_In_Alaska_DataStorytelling.png`

A `.twbx` is the best format to upload when you want other people to **open the workbook exactly as built** (dashboards, worksheets, formatting, calculations, filters, actions—and often the embedded extract/data too).

---

## What this folder contains

### 1) `.twbx` (Tableau Packaged Workbook)
- **Purpose:** Full reproducibility of the Tableau work
- **Includes (typical):**
  - Dashboards + worksheets
  - Calculated fields, parameters, sets
  - Filters, actions, tooltips, formatting
  - Data source info (and often an embedded extract)

> **Note:** If your `.twbx` was saved with an embedded extract, it will open without needing external CSV/Excel files.  
> If it was saved with a live connection, Tableau may ask you to locate the source file when opening.

### 2) Dashboard export image (reference)
- `Tableau_KingCrab_Population_In_Alaska_DataStorytelling.png`  
  Used as a quick preview of the final dashboard layout.

---

## Requirements to open the `.twbx`

You can open a `.twbx` using:

- **Tableau Desktop** (recommended for full editing)
- **Tableau Public (Desktop app)** (works for viewing/editing, then publishing to Tableau Public)

### Recommended setup
- Use a modern Tableau version (ideally the same or newer than the one used to create the workbook).
- If you get compatibility warnings, choose **“Open anyway”** and then re-save.

---

## How to open (step-by-step)

1. Download the `.twbx` file from this folder to your computer.
2. Double-click it, or open Tableau → **File → Open** → select the `.twbx`.
3. If Tableau prompts for data:
   - Click **Edit Connection** or **Locate File**
   - Point Tableau to the required data file location (only if the data wasn’t embedded).
4. Wait for the workbook to load (large `.twbx` files may take a bit longer).
5. Open the dashboard tab(s) at the bottom to view the final layout.

---

## How to navigate the dashboard (what to check first)

When the workbook opens, use this order to understand the story quickly:

1. **Filters / Controls**
   - Use filters (e.g., group/sex/year) to see how the full dashboard responds.
2. **Top-level KPI / summary visuals**
   - Identify the headline patterns first (counts, averages, totals).
3. **Relationships**
   - Check relationship plots (e.g., scatter/trend) for correlation patterns and outliers.
4. **Time-based change**
   - Inspect trend lines for growth/decline patterns across years.
5. **Group comparisons**
   - Compare segments side-by-side using bars/stacked bars.

---

## Exporting (so you can regenerate images anytime)

### Export the dashboard as an image (PNG)
1. Go to the dashboard tab.
2. **Dashboard → Export Image**
3. Set:
   - **Resolution:** High (if available)
   - **Scaling:** Fit entire view
4. Export and save.

### Export as PDF (for reports)
1. **File → Export as PDF**
2. Choose:
   - **Layout:** Landscape (usually best for dashboards)
   - **Scaling:** Fit to page
3. Export.

---

## Editing guidance (safe workflow)

If you want to adjust visuals without breaking layout:

### Best practice edits
- Update titles/subtitles for clarity
- Standardise fonts and number formatting
- Align containers and spacing
- Improve tooltip clarity
- Apply consistent colour rules

### Avoid (unless you intend to redesign)
- Removing key filters used across multiple sheets
- Changing aggregation levels (can alter meaning)
- Changing data joins/relationships without checking row counts

---

## Troubleshooting

### “Cannot locate file / data source missing”
- This happens when the workbook uses a live connection and the source isn’t embedded.
- Fix:
  1) Click **Edit Connection**  
  2) Use **Browse** to point Tableau to the correct file  
  3) Save the workbook again as `.twbx` (with extract embedded if needed)

### “Version compatibility” warning
- Open it in the newer Tableau version and re-save.

### Workbook loads but visuals are blank
- Click **Data → Refresh All Extracts**
- Or check filters aren’t excluding all values.

---

## Repository best practice notes (important)

### If the `.twbx` file is large
GitHub has practical limits for file uploads. If your `.twbx` is big (commonly 100MB+), use **Git LFS**.

**When to use Git LFS**
- The `.twbx` is too large to push normally
- You want clean versioning without failed uploads

**Git LFS files to track**
- `*.twbx`
- `*.hyper` (Tableau extracts)
- `*.tde` (older extracts)

---

## Suggested commit format for updates to the `.twbx`

**Commit title:**
- `Add Tableau packaged workbook (.twbx)`
or
- `Update Tableau packaged workbook (.twbx)`

**Extended description (example):**
- Added/updated Tableau packaged workbook in `assets/docs/` for reproducibility
- Preserves dashboards, worksheets, calculations, filters/actions as built
- Supports regeneration of `Tableau_KingCrab_Population_In_Alaska_DataStorytelling.png`
- Includes layout and logic for future iteration and review

---

## Quick file checklist (before uploading)

- [ ] Filename unchanged (as exported)
- [ ] Workbook opens successfully on your machine
- [ ] Dashboard tabs load correctly
- [ ] Filters work as expected
- [ ] Export image matches: `Tableau_KingCrab_Population_In_Alaska_DataStorytelling.png`

---
