---
title: Problem and Requirements
summary: Problem and Requirements document that will drive the work to be done in the project
date: "2018-06-28T00:00:00Z"
editable: true
share: false
---

## Target for the Semester

1. Outlier detection: 
    - KNN: This issue aims to explore how KNN works for timeseries data especially on paleoclimate data. Moreover, we also implement automate auto-tuning of the parameters using the silhouette method to heuristically determine all parameters
2. Visualization
    - SciencePlots: API for developing standardized plot styles using MatPlotLib (plots for IEEE, science, nature articles)
    - BoxPlots: This issue contends with the use pandas and Plotly to represent change in paleoclimatic data over the course of decades through the use of box plots to measure change in Southern Oscillation Index value
3. Fluctuation Analysis
    - HAAR: Current Pyleoclim Time Series analysis are effective yet costly due to our data’s characteristics. Haar Analysis improves the efficiency, forecasting quality, and particularly useful for data compression and denoising applications. Implement a working Haar Fluctuation Analysis Method for our data based on previous research algorithms created for similar data.

## Approach

1. Outlier detection
    - KNN on anomaly detection:
        - For KNN on anomaly detection, it involves identifying data points that deviate significantly from the majority of the data
        - KNN: Leveraging sklearn LocalOutlierFactor() function
        - Silhouette method: A metric used to assess the quality of clustering, we’re using it to evaluate the performance of models
 
2. Visualization
    - SciencePlots Functionality: 
        - Generate notebook with Pyleoclim/SciencePlot plot comparisons (IP)
        - Add SciencePlots into Pyelo dependencies and environment (IP)
        - Append new SciencePlot styles to Pyleo Plot.py file
        - Create Unit Test to ensure smooth integration of Scienceplots
        - Develop Scienceplots PyleoTutorial
    - Box plots for Time Series Data
        - Use .astype function of pandas to group points from the same year into one dataset
        - Generate boxplot using Plotly to juxtapose each year’s data and measure annual changes in the Southern Oscillation Index value

3. Fluctuation Analysis
    - Haar Fluctuation Analysis:
        - Determine notation and good defaults values for our method
        - Incorporate haar_v2 in Pyleoclim as a method of the Series class
        - Use this method to reproduce a findings similar to past research  on some of Pyleoclim’s pre-defined timeseries
        - Figure out a good unit test for this method
        - Implement it

## Use Case Scenario

- KNN on anomaly detection
![KNN](KNN.png)

- SciencePlots Functionality
![SciencePlot](SciencePlot.png)

- Box plots for Time Series Data
![BoxPlot](BoxPlot.png)

- Fluctuation Analysis
![HAAR](HAAR.png)