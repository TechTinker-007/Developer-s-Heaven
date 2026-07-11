# Changelog

All notable changes to this project are documented here.
Format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased] / Planned

### Planned
- Merge "Log a material delivery" and "Log usage" into a single unified entry bar
- Custom unit creation ("+ Add new unit") in the Unit dropdown with persistent save
- Supplier name attribution on min/max unit price rows in Suppliers tab
- Real-time budget threshold alert (in addition to the static over-budget banner)
- Expected-delivery-date notifications (bell icon + Alerts tab)
- Performance optimization: reduce lag/buffering on add, delete, and log usage actions
- Application-wide security hardening pass (RLS audit, input sanitization, rate limiting, session handling)

---

## [1.2.0] — Visual Analytics Expansion

### Added
- **Spend trend over time** chart (cumulative spend line)
- **Cost share by material** donut chart
- **Material-wise cost distribution** bar breakdown
- **Quantity delivered vs. used** grouped bar chart
- **Supplier price comparison** bar chart
- Reorganized Visual Analytics layout into overview → breakdown → drill-down hierarchy

---

## [1.1.0] — Suppliers Module

### Added
- Suppliers tab with "Spend by supplier" table (entries, total spend)
- "Price range across suppliers" table (min/max unit price per material)
- "Unspecified" supplier grouping for entries without a listed supplier

---

## [1.0.0] — Initial Release

### Added
- Project-based Material Log with delivery and usage entry forms
- Live Stock tracking per material
- Total Summary with budget vs. spend and over-budget banner
- Bulk entry support for deliveries
- CSV export and Print/PDF support for the Material Log
- Admin authentication (login/logout)
- Base Visual Analytics with unit price over time and cost share by material

---

[Unreleased]: #
[1.2.0]: #
[1.1.0]: #
[1.0.0]: #
