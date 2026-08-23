# PIUS Ltd Monthly Stock Dashboard

A lightweight, interactive **HTML stock dashboard** for tracking stationery and consumables inventory.

Built for **PIUS Ltd** stock counting and inventory reporting. Works entirely offline in any modern browser — no server or installation required.

**Author:** Paison Tazvy

## Features

- **KPI cards** for stock value and quantity:
  - Closing Stock Value
  - Net Change in Stock Value
  - Value Received / Issued
  - Total Quantity (Opening → Received → Issued → Closing)
- **Expandable category breakdown** — click a category to see individual stock lines
- **Watchlist** for Slow Moving, Marked for Disposal, and Out of Stock items
- **Editable Period** field (type any month/period)
- **Load new data** via CSV file picker
- Fully self-contained (data embedded + CSV support)
- Responsive layout

## How to Use

### View the dashboard
1. Download or clone this repository
2. Open `index.html` in Chrome, Edge, or Firefox (double-click the file)

### Update with new monthly data
1. Prepare a CSV file with these columns:

```
sn,description,unit,opening_qty,opening_unit_price,opening_value,received_qty,received_unit_price,received_value,issued_qty,issued_unit_price,issued_value,closing_qty,closing_unit_price,closing_value,status
```

2. Open the dashboard → click **Choose stock_data.csv** → select your new file
3. Update the **Period** field at the top (e.g. `Dec-2024`)

A sample file `stock_data.csv` is included.

## Project Structure

```
pius-stock-dashboard/
├── index.html          # Main dashboard (self-contained)
├── stock_data.csv      # Sample data
├── LICENSE
└── README.md
```

## Technical Notes

- Pure HTML + CSS + JavaScript (no frameworks)
- Data can be embedded or loaded from CSV
- Category grouping is automatic based on item description keywords
- Designed for internal reporting use

## Author

**Paison Tazvy**

## License

MIT License — feel free to use and adapt.
