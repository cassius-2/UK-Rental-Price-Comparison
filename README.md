# UK-Rental-Price-Comparison

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![UI/UX](https://img.shields.io/badge/UI/UX_Design-FF4F8B?style=for-the-badge)

## Overview
An end-to-end Power BI dashboard analysing the UK private rental market using official ONS data. This tool allows users to explore rental price trends across the last decade (2015-2026), categorised by region, local area, and property size.

Watch the quick demo here: **[https://1drv.ms/v/c/370a9c539f5269d7/IQAs8Jix4TMsRZ81Ko3szZkVAZU_7ksKS9ixOoaoI-YTWJg?e=j5WEPG]**

Note: Due to not having a Power Bi License, the demo is being shown on the desktop app so is not as smooth as it would be if it was published.

## Key Features & Technical Highlights

This dashboard moves beyond standard drag-and-drop visuals, employing Power BI techniques to deliver an app-like experience:

* **Dynamic UI (Bookmarks & Selections):**
    * Custom **Filter Selection Pane** utilising bookmarking for clean canvas management.
    * Global action buttons including a "Remove All Filters" reset and a dedicated "Default 2026 View" reset.
* **Context Specific Titles:**
    * **Dynamic Dashboard Headers:** The main title automatically updates via DAX to reflect the specific year currently filtered.
    * **Dynamic Visual Titles:** Main bar chart header Updates to reflect the parameter selected in the view slicer (e.g. Region, Year, or House Size).
* **Advanced Tooltips:**
    * Replaced default hover states with **Custom Report Page Tooltips**. Hovering over an area reveals a secondary chart detailing the Top 5 most expensive and Top 5 cheapest areas within that specific region, year or house size.
* **Dynamic Benchmarking & Aggregation:**
    * **Dynamic Callout Cards:** DAX measures automatically identify and display the single most expensive and cheapest areas based on the active filter context.
    * **Proportional Analysis Doughnut:** A dynamically calculating chart that evaluates the active subset of areas and splits them into "Over" or "Under" the fluctuating UK Average, reacting to House Size or Year adjustments.

## Concepts Demonstrated
* Evaluation Measures (`CALCULATE`, `ALLSELECTED`, `VALUES`)
* Virtual Table Iteration (`MINX`, `FILTER`)
* Field Parameters for dynamic axes
* Advanced Bookmark state management
* Custom UI Theme JSON configuration (Urban Slate & Terracotta)

## Data Source
* Office for National Statistics (ONS): Price Index of Private Rents
