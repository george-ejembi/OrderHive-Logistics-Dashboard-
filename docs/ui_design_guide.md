# Excel UI/UX Design Guide

This dashboard was designed to mimic a modern Business Intelligence tool (like Power BI or Tableau) entirely within Microsoft Excel. Here are the design techniques used:

### 🎨 Color Palette
- **Background:** `#1A1A1A` (Dark Grey/Black)
- **Cards:** `#FFFFFF` (White)
- **Primary Text:** `#000000` (Black)
- **Highlight Color:** `#ED7D31` (Orange)
- **Muted Text:** `#7F7F7F` (Grey)

### 🛠️ Excel Techniques Used
1. **Gridline Removal:** View -> Uncheck "Gridlines" to create a blank canvas.
2. **Shape Layering:** Used rounded rectangles behind charts to create "KPI Cards." Removed shape outlines and added subtle drop shadows for depth.
3. **Dynamic Text Boxes:** Used formulas inside text boxes (e.g., `="Total Orders: "&TEXT(B2,"0.00K")`) to display dynamic KPI numbers that update with slicers.
4. **Custom Charts:** 
   - Removed all chart borders and background fills.
   - Changed data series fill colors to match the dark theme.
   - Used combo charts (Bar + Line) to correlate order volume with delivery times.
5. **Slicers:** Used Form Control Slicers (Driver Name) instead of standard dropdowns for a cleaner, app-like feel. Adjusted slicer styles to match the dark theme.
6. **Iconography:** Used custom SVG icons or simple shapes to indicate metrics (e.g., the stopwatch for delivery times, the gear for processing times).
