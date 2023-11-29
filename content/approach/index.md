---
title: Approach
summary: Data science methodology used to address the problem, including data preprocessing steps, exploratory data analysis, feature engineering techniques, machine learning models, and evaluation metrics.
date: "2018-06-28T00:00:00Z"
editable: true
share: false
---

## Outlier detection
Before implementing KNN into Pyleoclim, we first did some [test](https://github.com/KnowledgeCaptureAndDiscovery/autoTS/blob/master/notebooks/Methods/Outlier/LOF.ipynb) on how KNN works for outlier detection. The tests includes using KNN outlier detection on several different datasets and exploring parameters of it:
1. Synthetic dataset
2. Real-world dataset
3. Explore KNN parameters
4. Timeseries dataset
5. Paleoclimate series

Next, we try simulating the new functionality in a separate [notebook](https://github.com/KnowledgeCaptureAndDiscovery/autoTS/blob/master/notebooks/Methods/Outlier/LOF_test.ipynb) before implemeting into the pyleoclim package.

Last, we modify the pyleoclim package, set up tests associated to the new functionalities, and [merge](https://github.com/LinkedEarth/Pyleoclim_util/commit/512c92d619ac692b2209f4a600c681db45e1a99e) the changes to the main branch.

## Visualization
### SciencePlot

### BoxPlot


## Fluctuation Analysis


