# Association Rule Generation from Transaction Data

This repo involves generating association rules from a transaction dataset using various support and confidence thresholds. The steps include downloading the dataset, extracting association rules, experimenting with different parameter values, and visualizing the results.

## Table of Contents

1. [Overview](#overview)
2. [Instructions](#instructions)
3. [Results](#results)
4. [Repository Structure](#repository-structure)
5. [How to Run the Notebook](#how-to-run-the-notebook)

## Overview

In here, I analyzed a transaction dataset to uncover interesting relationships between items using association rule mining. The analysis is performed with different minimum support and confidence thresholds, and the results are visualized using heatmaps.

## Instructions

1. **Download the transaction dataset:**
    - Download the Grocery_item.csv data.

2. **Extract association rules:**
    - Use a minimum support of 0.01 and a minimum confidence threshold of 0.1.
    - Refer to the [mlxtend documentation on association rules](http://rasbt.github.io/mlxtend/user_guide/frequent_patterns/association_rules/).

3. **Experiment with different parameters:**
    - Minimum support values: 0.001, 0.005, 0.01
    - Minimum confidence thresholds: 0.05, 0.075, 0.1
    - For each pair (msv, mct), find the number of association rules extracted from the dataset.
    - Construct a heatmap using the Seaborn library to visualize the results. The x-axis represents msv, and the y-axis represents mct. Refer to the [Seaborn heatmap documentation](https://seaborn.pydata.org/generated/seaborn.heatmap.html).

4. **Split the dataset and extract rules:**
    - Split the dataset into two equal subsets.
    - Extract association rules for each subset using a minimum support of 0.005 and a minimum confidence threshold of 0.075.
    - Identify which association rules appear in both subsets.

## Results

Detailed analysis and results can be found in the [Association_analysis.ipynb](Association_analysis.ipynb) Jupyter Notebook file.

## Repository Structure

- `Association_analysis.ipynb`: Jupyter Notebook containing the solution to the Association Rule Generation project.
- `data/`: Directory containing the datasets used in the project.
- `README.md`: This README file.

## How to Run the Notebook

1. Clone the repository to your local machine.
2. Ensure you have the required libraries installed. You can install the dependencies using:

   ```bash
   pip install -r requirements.txt
