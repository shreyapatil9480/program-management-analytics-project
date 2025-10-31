
# Program Management Analytics Project

This repository contains a synthetic dataset and analysis notebook for exploring project management and program analytics. It is designed for aspiring Business Analysts, Program Managers, and Data Analysts to practice end‑to‑end data analysis, from loading and cleaning data to visualizing relationships and building predictive models.

## Dataset

The dataset, **`synthetic_project_data.csv`**, contains 500 synthetic project records with the following columns:

| Column | Description |
|--------|-------------|
| `Project_ID` | Unique identifier for each project |
| `Team_Size` | Number of team members working on the project |
| `Complexity` | A rating of project complexity (1–9) |
| `Risk_Rating` | A rating of project risk (1–9) |
| `Scope_Creep_Frequency` | Number of scope‑change requests during the project |
| `Duration` | Project duration in arbitrary units (derived from team size and complexity) |
| `Budget` | Project budget in hypothetical currency units |
| `Client_Satisfaction` | Client satisfaction score (0–100) |
| `Success` | Binary indicator (1=success, 0=not) based on satisfaction and duration |

The values are generated synthetically and do not represent real projects. They are designed to resemble plausible project characteristics and outcomes.

## Analysis Notebook

The Jupyter notebook **`analysis.ipynb`** walks through a typical analytics workflow:

1. **Load the dataset** using `pandas`.
2. **Inspect and clean data**, checking for missing values and basic statistics.
3. **Exploratory Data Analysis (EDA)** with visualizations:
   - Distribution of key variables (e.g., budget, duration).
   - Correlation heatmaps to understand relationships between features.
   - Scatter plots to explore specific feature interactions.
4. **Predictive Modeling**:
   - A regression model (e.g., Random Forest Regressor) to predict `Client_Satisfaction`.
   - A classification model (e.g., Logistic Regression) to predict project `Success`.
   - Evaluation of model performance using appropriate metrics.

## Getting Started

To reproduce the analysis:

```bash
# Clone this repository
git clone <repository-url>
cd program-management-analytics-project

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scriptsctivate`

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook analysis.ipynb
```

Follow the notebook’s step‑by‑step analysis to explore the dataset and experiment with predictive models. You can modify parameters or models to see how they impact performance.

## Project Goals

- Demonstrate data preparation, visualization, and modeling in the context of project/program analytics.
- Provide a starting point for customizing more complex analyses, such as forecasting project success or analyzing risk factors.
- Showcase your analytical and storytelling skills on GitHub when applying for roles like Business Analyst, Program Manager, or Data Analyst.

## License

This project is provided for learning purposes under the MIT License. You are free to reuse and modify the content to suit your needs.
