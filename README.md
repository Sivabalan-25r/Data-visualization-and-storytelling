# Task 2: Data Visualization & Storytelling

## Objective
Build a set of visualizations from sales data that tell a clear business story,
using Power BI Desktop.

## Files in this repo
| File | Description |
|---|---|
| `superstore_sales.csv` | Sales dataset used (Region, Category, Sales, Profit, etc.) |
| `superstore_dashboard.pdf` | Exported dashboard (all charts) |
| `README.md` | This file |

## Tool Used
Power BI Desktop (free, Windows)

## Charts Built & Why
1. **Sales by Category (bar chart)** — compares 3 categories by total sales.
   Bar chosen over pie because bars make it easy to compare near-equal values precisely.
2. **Profit by Category (bar chart)** — placed next to Chart 1 to expose the mismatch
   between high sales and low profit in Furniture.
3. **Sales Trend Over Time (line chart)** — shows monthly sales movement;
   a line chart suits continuous time-series data better than bars.
4. **Profit by Region (bar chart)** — compares 4 regions; avoided pie chart since
   the four values are close and would be hard to distinguish as slices.
5. **Profit by Sub-Category (sorted bar chart)** — the sharpest insight chart;
   reveals that Tables/Bookcases underperform while Phones/Copiers drive profit.

## Key Insight (Headline)
**Furniture drives high sales volume but contributes very little profit,
while Technology sub-categories like Phones and Copiers are the real profit engine.**
Office Supplies, despite low sales, has a strong profit margin.

## Design Choices (Clutter & Color)
- Removed unnecessary gridlines
- Used a single accent color to highlight the lowest-performing sub-category,
  greyed out the rest so the eye goes to the right place first
- Each chart is titled with the **finding**, not just the field name
  (e.g. "Tables & Bookcases barely profit" instead of "Profit by Sub-Category")

## How to Reproduce
1. Open Power BI Desktop
2. Get Data → Text/CSV → load `superstore_sales.csv`
3. Rebuild the 5 charts as described above
4. File → Export → Export to PDF

## Key Learnings
- Chart type should match the data type: categories → bar, time → line,
  two numbers → scatter. Pie charts should only be used for 2-3 categories
  with clearly different sizes.
- A dashboard's power comes from **contrast** — putting Sales and Profit
  charts side-by-side revealed an insight neither chart shows alone.
- Titling charts with the takeaway (not the field name) is what turns a
  set of charts into a "story."
- Reducing clutter (gridlines, unnecessary legends, too many colors) makes
  the real insight easier to spot.
