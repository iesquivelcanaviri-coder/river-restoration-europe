# 🇦🇹 Emissions Restoration Modeling: Austria Case Study

This project analyzes pollutant emissions from manure management in Austria, focusing on arsenic (As) levels. It models a restoration scenario simulating a 30% reduction in emissions starting in 2025, providing insights into environmental policy impacts.

---

## Objective

To demonstrate how data-driven restoration modeling can inform environmental decision-making by:

- Filtering and analyzing emissions data for a specific country, pollutant, and sector  
- Simulating a restoration scenario with reduced emissions post-2025  
- Visualizing original vs. restored emissions over time  

This project is designed to showcase scientific rigor, reproducibility, and policy relevance — ideal for research institutions like CERN.

---

## Dataset

- **Source**: `emissions_data.csv`  
- **Format**: Tab-separated values (`.tsv`)  
- **Required Columns**:
  - `country`
  - `pollutantName`
  - `sectorName`
  - `year`
  - `value`

Ensure the dataset is placed in the root directory or update the path in `DATA_PATH`.

---

## Methodology

1. **Load & Validate**: Reads the dataset and checks for required columns  
2. **Filter**: Selects rows matching Austria, arsenic (As), and manure management  
3. **Clean**: Converts year and value to numeric, drops missing entries  
4. **Model**: Applies a 30% reduction to emissions from 2025 onward  
5. **Visualize**: Plots original vs. restored emissions using Seaborn  

---

## Output

- **Plot**: Line chart comparing original and restored emissions  
- **Console**: Summary of grouped emissions by year  
- **Optional**: Save results to CSV or image (can be added)

---

## 🚀 How to Run

```bash
python emissions_model.py
