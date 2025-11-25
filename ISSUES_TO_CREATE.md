# GitHub Issues to Create for Demo

Create these 6 issues manually on GitHub to demonstrate drift scenarios.

Go to: https://github.com/kevindunne1/prd-drift-detector-demo/issues/new

---

## Issue #1: CSV Export Feature (DELIVERED ✅)

**Title:** Implement CSV export for dashboard data

**Labels:** `feature`, `enhancement`

**Description:**
```
Implement CSV export functionality for the analytics dashboard.

**Requirements:**
- Export dashboard data to CSV format
- Include completion percentage, risk scores, and requirement details
- File naming: `export-{project}-{timestamp}.csv`
- Handle special characters and unicode properly

**Acceptance Criteria:**
- [x] User can click "Export to CSV" button
- [x] CSV file downloads with correct data
- [x] Special characters are escaped properly
- [x] File name includes timestamp

**Status:** Completed and deployed to production
```

**After creating, CLOSE this issue** (click "Close issue" button)

---

## Issue #2: PDF Export with Branding (PARTIAL SCOPE DRIFT ⚠️)

**Title:** Add PDF export with company branding

**Labels:** `feature`, `enhancement`

**Description:**
```
Enable PDF export of dashboard reports with company branding.

**Requirements (from PRD):**
- Export dashboard data to PDF format
- Include company logo in header
- Custom header/footer support
- Works in both light and dark mode

**What Was Delivered:**
- ✅ Basic PDF export functionality
- ✅ Standard header with project name
- ❌ Company logo not implemented (deferred to Phase 2)
- ❌ Custom header/footer not implemented

**Status:** Partially complete - basic PDF works but branding features missing

**Scope Drift:** PRD specified "PDF exports should include company logo and custom header/footer" but only basic PDF without branding was delivered.
```

**After creating, CLOSE this issue** (click "Close issue" button)

---

## Issue #3: Dashboard Visualization Improvements (IN PROGRESS 🔄)

**Title:** Build dashboard with completion gauge and risk indicators

**Labels:** `feature`, `enhancement`, `in-progress`

**Description:**
```
Implement visual dashboard components for analytics display.

**Requirements:**
- Completion percentage as gauge chart
- Risk scores with color coding (green/yellow/red)
- Timeline drift visual indicators
- Sortable requirements list

**Progress:**
- [x] Basic dashboard layout
- [x] Completion percentage display (numeric)
- [ ] Gauge chart visualization (in progress)
- [ ] Risk color coding
- [ ] Timeline drift indicators
- [ ] Sortable requirements list

**Status:** In active development, targeting completion next sprint
```

**Leave this issue OPEN**

---

## Issue #4: Date Range Filtering (DELIVERED ✅)

**Title:** Add date range filter for exports

**Labels:** `feature`, `enhancement`

**Description:**
```
Allow users to filter export data by date range.

**Requirements:**
- Filter options: Last 7 days, 30 days, 90 days, custom range
- Apply to both CSV and PDF exports
- Date range displayed in export file

**Acceptance Criteria:**
- [x] Dropdown with preset date ranges
- [x] Custom date picker
- [x] Filter applied to export data correctly
- [x] Date range shown in export metadata

**Status:** Completed and tested
```

**After creating, CLOSE this issue** (click "Close issue" button)

---

## Issue #5: Real-time Dashboard Refresh (SCOPE DRIFT ⚠️)

**Title:** Implement automatic dashboard refresh

**Labels:** `feature`, `enhancement`

**Description:**
```
Enable automatic refresh of dashboard data for live viewing.

**PRD Requirement:**
"Dashboard should update automatically every 30 seconds when viewing live data"

**What Was Delivered:**
Dashboard refreshes automatically every **60 seconds** (not 30s as specified)

**Reasoning:**
After performance testing, we found 30s refresh caused excessive API calls and impacted backend performance. Team decided on 60s refresh rate as a compromise between freshness and performance.

**Status:** Delivered with modified spec (60s instead of 30s)

**Scope Drift:** Refresh interval doubled from PRD specification
```

**After creating, CLOSE this issue** (click "Close issue" button)

---

## Issue #6: Access Control and Audit Logs (NOT STARTED ❌)

**Title:** Implement export access control and audit logging

**Labels:** `feature`, `security`, `phase-2`

**Description:**
```
Add access control and audit logging for export feature.

**Requirements:**
- Export feature respects user permissions (view-only cannot export)
- Audit log tracks all export actions (who, what, when)
- Exports with sensitive data require manager approval

**Status:** Not started - deferred to Phase 2

**Rationale:** Deprioritized to deliver core export functionality in Phase 1. Security team confirmed existing role-based access control provides adequate protection for initial release.
```

**Leave this issue OPEN**

---

## After Creating All Issues

Your demo repo will show:
- 4 closed issues (delivered features)
- 2 open issues (in-progress and not started)
- Mix of clean delivery, scope drift, and missing features

This gives the drift detector realistic scenarios to analyze.

**Create these issues now at:**
https://github.com/kevindunne1/prd-drift-detector-demo/issues/new
