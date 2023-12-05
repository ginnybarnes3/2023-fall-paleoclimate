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
One requested new feature for the Pyleoclim package was the implementation of SciencePlots in the plotting.py file so that plots created with Pyleoclim would fit science, ieee, nature, and notebook publication guidelines. In order to follow the guidelines, certain plot feature need to be set such as trendline colors, font, legend styles and more.

A notebook was created to show the comparison of the previous styles offered in Pyleoclim from matplotlib and the new styles implemented from SciencePlots which cam be found here:
https://github.com/ginnybarnes3/Pyleoclim_util_Barnes/blob/Barnes_Ginny_SciencePlots/PyleoSciencePlotsImplemented.ipynb
The file is too large to view on GitHub but the notebook can be downloaded and run on jupyter lab to view the comparisons.

### BoxPlot


## Fluctuation Analysis


