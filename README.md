# Data Science Experiment 1 - Loading and Merging Datasets

This repository contains the code and results for the first experiment in the Data Science Fundamentals with Python course. The objective of this experiment is to load and merge datasets obtained from the UCI Machine Learning Repository.

## Experiment Overview

### Steps:
1. **Loading Datasets**: The datasets are loaded using the Pandas library from the UCI ML Repository.
2. **Inspecting Datasets**: The first few rows of each dataset are displayed to understand their structure.
3. **Merging Datasets**: The datasets are merged on a common column (e.g., 'ID').
4. **Saving the Merged Dataset**: The merged dataset is optionally saved as a CSV file.

## Concepts Used
- **Pandas Library**: Used for data manipulation and analysis.
- **DataFrames**: Data structures provided by Pandas to store and manipulate tabular data.
- **Merging Datasets**: The `pd.merge()` function is used to combine two datasets based on a common key.

## Steps to Reproduce

1. **Set up Google Colab**:
   - Open [Google Colab](https://colab.research.google.com/).
   - Create a new notebook.

2. **Import Necessary Libraries**:
   - Start by importing the required libraries.

    ```python
    import pandas as pd
    ```

3. **Load the Datasets**:
   - Use the URL of the datasets from the UCI ML repository.

    ```python
    url1 = 'dataset_url_1'
    url2 = 'dataset_url_2'
    df1 = pd.read_csv(url1)
    df2 = pd.read_csv(url2)
    ```

4. **Inspect the Datasets**:
   - Show the first few rows of each dataset to verify they loaded correctly.

    ```python
    print("First dataset:")
    print(df1.head())
    
    print("\nSecond dataset:")
    print(df2.head())
    ```

5. **Merge the Datasets**:
   - Merge the datasets on a common column (e.g., 'ID').

    ```python
    merged_df = pd.merge(df1, df2, on='ID')
    ```

6. **Inspect the Merged Dataset**:
   - Display the first few rows of the merged dataset.

    ```python
    print("\nMerged dataset:")
    print(merged_df.head())
    ```

7. **Save the Merged Dataset**:
   - Save the merged dataset to a CSV file.

    ```python
    merged_df.to_csv('merged_dataset.csv', index=False)
    ```

## How to Use
1. Clone this repository.
2. Run the notebook `Experiment_1_AIDS_SUJAL_SOKANDE.ipynb` in Google Colab or locally.

## Dataset
The datasets used in this experiment are sourced from the [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/index.php).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
