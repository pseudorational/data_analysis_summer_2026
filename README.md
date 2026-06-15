# Data Analysis Workshops - Summer 2026

Welcome to the **Data Analysis Workshops - Summer 2026** repository! This repository contains course materials, Jupyter Notebooks, datasets, and exercises for mastering data exploration, transformation, and sharing using Python.

---

## 📂 Repository Structure

The workshop is organized into three sessions:

*   **`Session1_Explore/`**
    *   Covers Python programming basics, data structures, and core libraries like NumPy and Pandas.
    *   Includes introductory exercise notebooks.
*   **`Session2_Transform/`**
    *   Focuses on data cleaning, filtering, sorting, handling missing values, pivoting, and aggregation.
    *   Key notebook: `data_exploration.ipynb` (contains detailed tutorials on indexing, grouping, and light-weight data visualizations using built-in Pandas `.plot()` methods).
*   **`Session3_Share/`**
    *   Focuses on formatting, sharing analysis, and generating reports from data insights.

---

## 🛠️ Getting Started

### Prerequisites

To run these notebooks, you will need **Python 3.10+** along with the following data analysis libraries:
*   [Pandas](https://pandas.pydata.org/)
*   [NumPy](https://numpy.org/)
*   [Matplotlib](https://matplotlib.org/)

You can install these dependencies using `pip`:
```bash
pip install pandas numpy matplotlib notebook
```

### Running the Notebooks

1. Clone or download this repository.
2. Launch Jupyter Notebook from your terminal:
   ```bash
   jupyter notebook
   ```
3. Navigate to any of the session folders and open the `.ipynb` files to begin.

---

## 📈 Visualizations in `data_exploration.ipynb`

In accordance with Python data science best practices, the visualization code in `Session2_Transform/data_exploration.ipynb` has been designed to use built-in Pandas `.plot()` methods (built on top of Matplotlib). This keeps the visualization code extremely light-weight and easy to read.

Examples include:
*   **Histogram of Market Cap:** `df['market_cap'].plot(kind='hist')`
*   **Horizontal Bar Charts:** `df.groupby('headquarters_state')['market_cap'].mean().plot(kind='barh')`
*   **Scatter Plots:** `df.plot(x='revenue', y='market_cap', kind='scatter')`
