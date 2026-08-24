# Stock-Maintenance-System
A Stock Maintenance System is a software application used to manage and monitor inventory efficiently. It records stock details, purchases, sales, and stock movements. It helps track available quantities, identify low-stock items, reduce errors, avoid shortages, and generate reports for effective inventory management and decision-making.
This project is created for academic demonstration purpose only
Software Configuration Management using GitHub.
Student Name: D Hemanth 
Roll Number: 25B81A6678
Class: 2nd year 1st sem btech


## Requirements

### 1) Summary / Purpose
- Lightweight system to manage inventory: record items, purchases, sales, stock movements, low-stock alerts, simple reporting and import/export for backups. Works as a single-page client app (localStorage) or with optional server persistence.

### 2) Actors / User Roles
- Guest / Clerk: Add/edit/delete items, perform purchases/sales, view inventory and reports.
- Manager: Same as Clerk + import/export, adjust low thresholds, run reports.
- Admin (optional): Manage users, roles, and system settings, backup/restore.

### 3) Functional Requirements (Must-have)
- Item CRUD: Create, read, update, delete items with fields: id, name, SKU, price, quantity, low-stock threshold, optional description/category.
- Stock adjustments: Record purchase (increase) and sale (decrease) with quantity prompts and safeguards.
- Search, sort, filter: Search by name and SKU, sort by columns, filter by low-stock or category.
- Low-stock indication: Highlight items at/below threshold and provide low-stock list.
- Data persistence & import/export: LocalStorage baseline, CSV export/import with merge policy.
- Totals & summary: Show item count and total inventory value.
- Usability: Form validation, edit-in-form, reset/clear.

### 4) Non-functional Requirements
- Responsive UI, performant for large lists (pagination/virtualization beyond ~2000 items), offline availability (localStorage), accessibility, and maintainability.

### 5) Data Model (minimum fields)
- id (string), name (string), sku (string), description (string), category (string), price (decimal >=0), qty (integer >=0), lowThreshold (integer >=0), lastUpdated (timestamp), createdAt (timestamp).

### 6) UI / UX Requirements
- Two-pane layout (form + inventory list), inline row actions (purchase/sale/edit/delete), search and sort, clear import/export controls, low-stock visual indicator, confirmations for destructive actions.

### 7) Security & Privacy (if extended with server)
- Authentication, authorization, HTTPS, input validation, rate limiting, and controlled backups.

### 8) Reporting & Backup
- CSV export, printable reports (low-stock, inventory value), optional audit trail for adjustments.

### 9) Integrations (optional)
- Barcode scanning, Excel import, cloud sync.

### 10) Error handling & constraints
- Graceful error messages for import/storage errors, validation to prevent invalid entries, defined import merge policy for duplicates.

### 11) Testing & Acceptance Criteria
- Add/Edit/Delete persist across reloads; purchase/sale update quantities and totals; low-stock highlight active; CSV import/export functional; search and sort work; form validation enforced.

### 12) Documentation & Deliverables
- README (this file) with setup/usage, sample CSV, front-end source files (index.html, styles.css, app.js), and optional server API docs and tests.

### 13) Nice-to-have / Future Enhancements
- Authentication, audit trail, server-side persistence (Node/Express + SQLite), bulk edit, scheduled alerts, dashboard charts, mobile/PWA support.

### 14) Suggested Tech Stack
- Minimal: HTML/CSS/Vanilla JS + localStorage. With backend: Node.js + Express + SQLite/Postgres. Front-end upgrade: React/Vue.

### 15) Development Plan & Milestones
- Day 1: Wireframes & UI, Day 2: CRUD + persistence, Day 3: search/sort/low-stock, Day 4: CSV import/export, Day 5: tests/documentation. + Additional days for server/auth.

### 16) Assumptions & Constraints
- Baseline single-user client-side; CSV import expects header row; SKU uniqueness recommended but not enforced by baseline implementation.


<!-- Commit: Added project requirements -->
