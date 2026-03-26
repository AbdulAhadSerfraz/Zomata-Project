# Zomata Data Analysis

A complete exploratory data analysis project for Zomato dataset, built in Jupyter Notebook.

## Project Goals

- Identify top restaurant types by volume and votes
- Visualize rating distribution across dataset
- Compare online vs offline order ratings and order counts
- Calculate average couple spending for online orders
- Understand restaurant-type vs online/offline order mix

## Files in this repository

- `Zomata Data Analysis.ipynb` - main analysis notebook
- `Zomato data .csv` - training dataset used for analysis
- `.gitignore` - ignores notebook checkpoints and temporary files

## How to run

1. Clone repository
2. Open in VS Code / Jupyter
3. Ensure dependencies are installed:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
4. Run notebook cells sequentially.

## Key insights

- `Dining` is the most frequent restaurant type and has the highest votes.
- Most restaurants have ratings clustered around 3.5 to 4.0.
- Online orders have higher average ratings than offline orders.
- Average couple spending for online orders is around 310 (currency as per dataset).
- Dining has the highest overall volume; Cafes/Other show strong online share.

## Next improvements

- Add data validation (missing values, invalid rates)
- Add pairwise correlations and hypothesis testing
- Create aggregated KPI dashboard with Streamlit or Plotly

## License

MIT License
