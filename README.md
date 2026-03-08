# Predicting-Life-Expectancy

This repository contains a project focused on predicting life expectancy using machine learning techniques like regression, feature selection, regularization. The project includes data inspection, exploratory data analysis (EDA), and the development of predictive models to estimate life expectancy based on various features.

## Dataset
The dataset can be found here: [Life Expectancy Data](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who).

## Project Structure

```text
Predicting-Life-Expectancy/
├── data/                   # Data directory (raw and processed data)
│   ├── raw/                # Original data downloaded from Kaggle
│   └── processed/          # Cleaned data ready for modeling
├── notebooks/              # Jupyter notebooks for exploration and preprocessing
│   ├── 01_data_inspection_and_EDA.ipynb
│   └── 02_data_preprocessing.ipynb
├── src/                    # Source code for scripts and modules
│   ├── preprocess.py       # Data preprocessing scripts
│   └── utils.py            # Shared utility functions
├── models/                 # Trained and serialized models
├── reports/                # Generated analysis, reports, and figures
├── environment.yml         # Conda environment specifications
└── README.md               # The top-level README for developers using this project
```

## Setup & Installation

This project uses `conda` to manage its environment and dependencies. To set up the project on your local machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd Predicting-Life-Expectancy
   ```

2. **Create the Conda environment:**
   Use the provided `environment.yml` file to create a virtual environment with all required dependencies.
   ```bash
   conda env create -f environment.yml
   ```

3. **Activate the environment:**
   ```bash
   conda activate venv
   ```
   *(Note: Based on your `environment.yml`, the environment may be created at a specific path. Check the output of the create command for the exact activation instruction).*

## Usage

1. **Data Preparation:** 
   - Download the dataset from the Kaggle link provided above.
   - Place the downloaded dataset in the `data/raw/` directory.

2. **Analysis and Preprocessing:**
   - Open Jupyter Notebook `jupyter notebook` in your activated environment.
   - Run through `notebooks/01_data_inspection_and_EDA.ipynb` to explore the data, check for missing values, and visualize distributions.
   - Run through `notebooks/02_data_preprocessing.ipynb` to clean the data and prepare it for training.

3. **Source Scripts:**
   - The `src/` directory contains Python scripts (`preprocess.py`, `utils.py`) which can be used to run data processing pipelines or utility functions programmatically.

## Visualizations
Various visualizations (such as scatterplots, boxplots, correlation heatmaps, etc.) are generated during the EDA phase. These are saved in the root or `reports/` directory to help understand the characteristics of the dataset and how different features correlate with Life Expectancy.