# Sales Data Analysis Notebook

This Jupyter notebook performs comprehensive exploratory data analysis on apparel sales data, focusing on seasonal trends, material performance, product positions, promotions impact, and price-sales relationships. Key visualizations reveal Autumn as the peak sales season and jackets as top performers.

# Report

### *View the full report:* [🛍️ Zara Sales Report](https://zara-sales-report.notion.site/ebd//2d59f5e250fa8099a17cfd70d7e51ccd)

# Features

- Seasonal sales analysis showing Autumn dominance followed by Winter
- Material breakdown with Polyester and Cotton leading sales
- Product position effects (Aisle, End-cap, Front of Store) and promotion boosts
- Section-wise performance (Womens, Mens) and top products like jackets
- Price-sales volume correlations (-0.33 overall, similar for jackets/sweaters)
- Interactive Plotly visualizations for all analyses

## Project Structure

```
data/                   # Add your sales CSV here
    ├── raw/              # Original dataset
    └── processed/        # Cleaned data
notebook/
    └── Analysis.ipynb  # Main analysis notebook with all code and visuals
README.md
requirements.txt
```

## Requirements
Execute the following command to install requirements.txt:

```bash
pip install -r Zara-Sales-analysis/requirements.txt
```


## Quick Start

1. To run ipykernel, run the following command:
    ```bash 
    jupyter lab --no-browser
    ```
    Note: running `ipykernel` and selecting it specifically instead of python interpreter is important to run the `Analysis.ipynb` notebook properly.
2. Open `Analysis.ipynb` and run all cells sequentially.
3. View interactive charts and insights immediately.

**Expected runtime**: ~2 minutes on standard hardware.

## Key Insights

| Analysis | Finding | Visualization |
|----------|---------|---------------|
| Seasonal Sales | Autumn > Winter > Spring > Summer | Bar chart by Season |
| Top Materials | Polyester, Cotton dominate | Histogram |
| Promotions Impact | +7.3% overall sales volume boost | Stacked bar by Product Position |
| Top Products | Jackets lead across seasons | Seasonal product histogram |
| Gender Breakdown | Womens products dominate purchases | Section vs Products chart |
| Price Correlation | -0.34 (negative) with sales volume | Scatter plot + correlation stats |

## Data Requirements

The notebook expects a CSV with these columns:

- `Season`: Spring, Summer, Autumn, Winter
- `Sales`: Numeric sales values
- `Sales Volume`: Unit quantities
- `Material`: Polyester, Cotton, Wool Blend, etc.
- `Product Position`: Aisle, End-cap, Front of Store
- `Promotion`: Yes/No
- `Products`: jackets, sweaters, shoes, etc.
- `Section`: WOMAN, MAN (Womens, Mens)
- `Price`: Numeric price per unit

## Outputs Generated

- Correlation statistics printed in notebook
- Summary tables for top materials/products/seasons

---
