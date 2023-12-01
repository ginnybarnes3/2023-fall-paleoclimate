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

Repository with code to compare different styles: https://github.com/ginnybarnes3/Pyleoclim_util_Barnes/blob/Barnes_Ginny_SciencePlots/PyleoSciencePlotsImplemented.ipynb
When opened in Jupyter Lab and run, displayes various plots using the 'journal' style from matplotlib, and the 'science', 'ieee', 'nature', and 'notebook' styles from SciencePlots.

These styles have been integrated in to Pyleoclim in this fork and can be used to plot various datasets. Additional features can be added to change the colors and of the displays and more.

Next, tests will be developed to ensure the SciencePlots feature will integrate well with the Pyleoclim package.

For users:
When creating a plot, one sets the style with the following line of code:
  pyleo.utils.plotting.set_style(style= styleType, font_scale=1.0, dpi=300)
where styleType can be various styles such as 'science', 'ieee' etc.
It is a very simple integration to adapt plots for certain types of publications.


### SciencePlot

### BoxPlot


## Fluctuation Analysis


