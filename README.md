# STA-141A-Course-Project

## Project Overview
This repository contains the final project for STA 141A, focusing on a subset of data collected by Steinmetz et al. (2019). In the study, the experiments were performed on a total of 10 mice over 39 sessions. Each session comprised several hundred trials, during which visual stimuli were randomly presented to the mouse on two screens positioned on both sides of it. The stimuli varied in terms of contrast levels, which took values in {0, 0.25, 0.5, 1}, with 0 indicating the absence of a stimulus. The mice were required to make decisions based on the visual stimuli, using a wheel controlled by their forepaws. A reward or penalty (i.e., feedback) was subsequently administered based on the outcome of their decisions. In particular,

- When left contrast > right contrast, success (1) if turning the wheel to the right and failure (-1) otherwise.
- When right contrast > left contrast, success (1) if turning the wheel to the left and failure (-1) otherwise.
- When both left and right contrasts are zero, success (1) if holding the wheel still and failure (-1) otherwise.
- When left and right contrasts are equal but non-zero, left or right will be randomly chosen (50%) as the correct choice.

The activity of the neurons in the mice’s visual cortex was recorded during the trials and made available in the form of spike trains, which are collections of timestamps corresponding to neuron firing. In this project, we focus specifically on the spike trains of neurons from the onset of the stimuli to 0.4 seconds post-onset. In addition, we only use 18 sessions (Sessions 1 to 18) from four mice: Cori, Frossman, Hence, and Lederberg.The project involves analyzing [data description] using R, employing various statistical and visualization techniques to uncover meaningful insights.

This project involves analyzing this dataset using R, implementing data cleaning, exploratory data analysis, statistical modeling, and visualization techniques to derive insights.

## Methodology
1. Data Collection & Preprocessing
- Imported the datasets using readr and tidyverse.
- Cleaned and transformed data by handling missing values, filtering out irrelevant entries, and restructuring variables for analysis.

2. Exploratory Data Analysis (EDA)
- Generated summary statistics to understand data distribution and key attributes.
- Created visualizations using ggplot2, including histograms, scatter plots, and box plots, to identify patterns and outliers.

3. Statistical Modeling & Analysis
- Applied regression analysis and hypothesis testing where applicable.
- Implemented machine learning models or statistical tests to validate findings.
- Used cross-validation techniques to assess model performance.

4. Visualization & Interpretation
- Developed detailed plots and graphs to illustrate trends and correlations.
- Interpreted results and contextualized findings within the scope of the study

The project is split up into 3 parts:
- Part 1: Exploratory data analysis
i) Data structures across sessions (e.g., number of neurons, number of trials, stimuli conditions, feedback types)
ii) Neural activities during each trial
iii) Exploring the changes across trials,
iv) Homogeneity and heterogeneity across sessions and mice

- Part 2: Data integration
i) Proposing an approach to combine data across trials by extracting the shared patterns across sessions
ii) Addresses the differences between sessions

- Part 3: Model training and prediction -> building a prediction model to predict the outcome (i.e., feedback types). The performance will be evaluated on two test sets of 100 trials randomly selected from Session 1 and Session 18, respectively.

## Requirements
To run the project, ensure you have the following installed:
- R (version 4.3.2or later)
- RStudio
- Required R packages: ggplot2, dplyr, tidyverse, readr, caret, tidymodels, and others listed in the RMarkdown file.

  ## How to Run
  Clone this repository: ```python
git clone https://github.com/Bwaj99/sta141a-course-project.git
  ```
