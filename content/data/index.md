---
title: Data Assessment
summary: Data Assessment Document that gives an overview of the data used for the project.

date: "2018-06-28T00:00:00Z"
editable: true
share: false
---

## Introduction

When implementing functionalities, we make use of several timeseries datasets, specifically paleoclimate datasets for testing.

## Data Overview and Examples

This is an example of a paleoclimate dataset (MD982181.Khider.2014):
![dataset_example](dataset_example.png)

## Data Accessibility

We leverage the Linked Paleo Data ([LiPD](https://cp.copernicus.org/articles/12/1093/2016/)) standard container and its associated utilities as the source of datasets.

Also, more datasets could be found in the pyeloclim repo [example_data folder](https://github.com/LinkedEarth/Pyleoclim_util/tree/d1462f45132496b2453c32a6133fd3938c4f84b0/example_data).

## Data Formats

Paleoclimate data could be in multiple formats, LiPD (.lpd) is not an obligatory entry point to Pyleoclim, low-level modules work on NumPy **arrays** or Pandas **dataframes**, so most Pyleoclim timeseries analysis functionalities can apply to these more common types as well.

## Data Challenges

Paleoclimate data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.