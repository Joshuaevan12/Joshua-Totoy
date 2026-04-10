# Google Sites Embed Code

This repository stores ready-to-embed HTML dashboards/forms for Google Sites.

Last Updated: April 10, 2026

## Repository Structure

- `embed-code/`: All embeddable HTML files
- `Readme.md`: Project documentation

## Active Embed Files

- `embed-code/admin-monitoring.html`
	- Admin monitoring dashboard using Google Sheets CSV data
	- Includes search, status filter, and newest-first sorting

- `embed-code/planning-monitoring.html`
	- Planning monitoring dashboard
	- Includes search, status filter, and newest-first sorting

- `embed-code/communications-documents-monitoring.html`
	- Communications documents dashboard
	- Uses worksheet metadata and gid-based loading for reliable per-page data mapping
	- Fixed tab/page behavior so each document page loads its own sheet data
	- Includes newest-first sorting with date parsing and row-order fallback

- `embed-code/communications-request-form-embed.html`
	- Google Form embed wrapper for communications requests
	- Responsive and style-consistent with the monitoring dashboards

- `embed-code/workschedule-approval.html`
	- Work Schedule Approval Monitoring dashboard
	- Uses row 1 as header by default (`headerRow=1` behavior supported)
	- Supports Approval Status column (for example: Pending, Approved, Rejected)
	- Newest entries appear first
	- Simplified single-page layout (Approval Pages and Current Page sections removed)

- `embed-code/pnr-quality-policy-tar-embed.html`
	- TAR quality policy embed page

- `embed-code/pnr-quality-policy-tron-embed.html`
	- TRON quality policy embed page

- `embed-code/HOME-EMBED-INSTRUCTIONS.md`
	- Usage notes for embedding pages in Google Sites

## Recent Updates

April 10, 2026: Standardized visual palette and responsive behavior across embeds:

`embed-code/admin-monitoring.html`
- Admin monitoring dashboard using Google Sheets CSV data
- Includes search, status filter, and newest-first sorting

April 10, 2026: Improved Google Sheets tab mapping reliability for communications dashboards:

`embed-code/communications-documents-monitoring.html`
- Uses worksheet metadata and gid-based loading for reliable per-page data mapping
- Fixed tab/page behavior so each document page loads its own sheet data

April 10, 2026: Added robust newest-first ordering logic across monitoring dashboards:

`embed-code/planning-monitoring.html`
- Planning monitoring dashboard
- Includes search, status filter, and newest-first sorting

April 10, 2026: Added stronger header-row and status-column handling for work schedule approvals:

`embed-code/workschedule-approval.html`
- Uses row 1 as header by default (`headerRow=1` behavior supported)
- Supports Approval Status column (for example: Pending, Approved, Rejected)

April 10, 2026: Updated work schedule approval layout to maximize table space:

`embed-code/workschedule-approval.html`
- Simplified single-page layout
- Removed Approval Pages and Current Page sections

April 3, 2026: Communications monitoring fixes and approval embed enhancements:

`embed-code/communications-documents-monitoring.html`
- Corrected Email Monitoring and Social Media page data loading
- Improved per-sheet fetch behavior for Google Sites embeds

`embed-code/workschedule-approval.html`
- Added initial approval monitoring embed with responsive dashboard layout

## Google Sites Notes

- If changes do not appear immediately in Google Sites, append a cache-busting query string to the embed URL (for example: `?v=2`).
- For approval monitoring, ensure the sheet has a valid header row in row 1 and the approval values are set in the status column.
