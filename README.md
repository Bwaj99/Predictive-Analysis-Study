# Neural Activity and Decision-Making in Mice

## Overview

This project explores how neural activity influences decision-making in mice performing a visual discrimination task. Using data from Steinmetz et al. (2019), I analyzed neural spike trains recorded from four mice as they respond to varying visual contrast levels. The goal is to develop a predictive model that classifies trial outcomes based on neural activity and stimulus conditions.

## Project Structure

- **Exploratory Analysis**: Understanding neural activity patterns and decision trends
- **Data Integration**: Combining sessions to improve model robustness
- **Predictive Modeling**: Implementing a Random Forest classifier to predict trial outcomes
- **Performance Evaluation**: Testing model accuracy across different sessions

## Key Findings

- Stronger neural responses correspond to higher contrast differences and better decisions
- Neural activity varies across sessions and mice, requiring normalization techniques
- A Random Forest classifier achieves 71.63% accuracy in validation, with improved accuracy in later sessions (up to 95.37% for Session 18)

## Technologies Used

- **Languages**: R, LaTeX
- **Libraries**: ggplot2, dplyr, tidyr, randomForest, caret
- **Data Format**: `.rds` files converted into `.csv` and `.json`

## Running the Code

- Download and open STA-141A-Final-Project.rmd
- Make sure you have RStudio and R 4.3.2 (or later) downloaded
- Run each code block in order for all plots to load
- Adjust file paths as needed

1. Install necessary R libraries
2. Load `.rds` session data, extract, and preprocess all 18 files
3. Run exploratory analysis scripts to visualize neural activity
4. Train and evaluate the Random Forest model
5. Validate predictions on test datasets

## References

- Steinmetz et al. (2019) - [Dataset Source](https://pubmed.ncbi.nlm.nih.gov/31776518/)

---

🔬 **Author**: Bharadwaj Tallapragada  
📅 **Date**: March 17, 2025  
