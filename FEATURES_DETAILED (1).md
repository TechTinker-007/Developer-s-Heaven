# Features — Detailed

Field-level and behavioral detail for every module in Developer's Heaven.

---

## 📦 Material Log

### Log a Material Delivery
Fields:
- **Delivery Date** — date picker, defaults to today
- **Expected By** — optional expected delivery date, used for delivery-date alerts
- **Material** — free text (e.g. "Cement OPC 53")
- **Quantity** — numeric
- **Unit** — dropdown (bag, kg, ton, m³, ft, load, pcs, litre)
- **Unit Price** — numeric, used to calculate total spend
- **Supplier** — free text; entries without a value default to "Unspecified" in supplier reporting
- **Add entry** — submits the delivery record
- **+ Bulk Entry** — allows logging multiple deliveries in one action

### Log Usage
Fields:
- **Date** — date of material consumption
- **Material** — free text, matched against delivery log for stock calculations
- **Qty Used** — numeric
- **Unit** — dropdown, same list as delivery
- **Log usage** — submits the usage record
- Validation: requires date, material name, and unit before submission

### Material Log Table
- Lists all delivery entries with Date, Expected By, Material, Quantity, Unit, Unit Price, Total (auto-calculated), Supplier
- Inline edit and delete actions per row
- Export to CSV and Print/PDF support

---

## 📊 Stock
- Displays live stock balance per material
- Calculated as: total delivered quantity − total used quantity (unit-aware)

---

## 🏢 Suppliers

### Spend by Supplier
- Table of all suppliers with entry count and total spend
- Entries without a specified supplier are grouped under "Unspecified"

### Price Range Across Suppliers
- Per material: number of distinct suppliers, minimum unit price, and maximum unit price
- *(Planned: supplier name attribution for which supplier gave the min/max price)*

---

## 💰 Total Summary
- Displays total budget vs. actual spend for the project
- Over-budget banner appears project-wide when spend exceeds budget, showing amount spent, budget, and percentage used

---

## 📈 Visual Analytics

| Chart | Description |
|---|---|
| **Spend trend over time** | Cumulative spend line chart across the project timeline |
| **Cost share by material** | Donut chart showing % of total spend per material |
| **Material-wise cost distribution** | Bar-style breakdown of the same cost share data |
| **Unit price over time** | Line chart of unit price fluctuation for a selected material |
| **Quantity delivered vs. used** | Grouped bar chart comparing delivered vs. used quantity per material |
| **Supplier price comparison** | Bar chart comparing unit prices between suppliers for a given material |

Charts are ordered: overview (spend trend, cost share) → breakdown (cost distribution, delivered vs. used) → drill-down (unit price over time, supplier price comparison).

---

## 🔔 Alerts
- Over-budget banner displayed at the top of the project view when spend exceeds budget
- Alerts tab intended to surface budget and delivery-related notifications
- *(Planned: live-triggered alert the moment budget threshold is crossed, and notifications when an "Expected By" date arrives without a logged delivery)*

---

## 🔐 Access & Project Structure
- Admin-based login/logout
- Projects list view; each project has its own isolated Material Log, Stock, Suppliers, Summary, Analytics, and Alerts

---

## 🧭 Planned Enhancements
- **Unified entry bar**: merge "Log a material delivery" and "Log usage" into a single card/tabbed interface without changing either form's underlying logic
- **Custom units**: "+ Add new unit" option in the Unit dropdown with inline save, persisted for future entries
- **Supplier-attributed price ranges**: show which supplier corresponds to the min/max unit price per material
- **Live alerts**: real-time budget threshold trigger and expected-delivery-date notifications (bell icon + Alerts tab)
- **Performance**: optimistic UI updates and targeted re-renders for add/delete/log actions to eliminate full-page lag
