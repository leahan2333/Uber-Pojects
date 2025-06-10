# Does Uber Complement or Substitute Public Transit?
## An Empirical Analysis of Transportation Platform Economics

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen.svg)]()

## 📋 Table of Contents
- [Overview](#overview)
- [Research Question](#research-question)
- [Key Findings](#key-findings)
- [Methodology](#methodology)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation & Usage](#installation--usage)
- [Results](#results)
- [Technical Details](#technical-details)
- [Policy Implications](#policy-implications)
- [Contributors](#contributors)
- [References](#references)

## 🔍 Overview

This research investigates the impact of ride-hailing services (specifically Uber) on public transit ridership across U.S. metropolitan areas from 2004 to 2015. Using comprehensive panel data from 545 transit agencies, we employ econometric methods to determine whether Uber acts as a substitute or complement to traditional public transportation.

The study contributes to the growing literature on platform economies and transportation policy, providing data-driven insights for sustainable urban mobility governance.

## ❓ Research Question

**Do services like Uber serve as a substitute for public transportation, drawing commuters away from buses and trains? Or do they act as a complement, expanding access to public transit by solving the last-mile problem?**

This question has significant implications for:
- Urban transportation planning
- Public transit funding and policy
- Regulatory approaches to ride-sharing platforms
- Sustainable mobility strategies

## 🎯 Key Findings

Our analysis provides **consistent evidence that Uber acts as a substitute for public transportation**:

### Primary Results
- **4.18% average decline** in monthly transit ridership following Uber's introduction
- **Statistically significant** at the 1% level across multiple model specifications
- **Robust** across different treatment variable definitions

### Heterogeneous Effects
- **High-population areas**: 7.2% decline in ridership
- **Low-population areas**: 4.4% decline in ridership
- **High gas price environments**: 3.3% decline
- **Low gas price markets**: No significant effect

### Policy Insights
- Cost-sensitive substitution behavior
- Stronger effects in urban, transit-dependent areas
- Need for integrated transportation planning

## 🔬 Methodology

### Analytical Framework
- **Panel Fixed Effects Regression** with agency and time fixed effects
- **Log-linear specification** allowing percentage interpretation
- **Multiple robustness checks** including subsample analyses

### Treatment Variables
1. **Binary Uber Presence** (`treatUberX`): Indicates operational presence
2. **Google Trends Intensity** (`treatGTNotStd`): Continuous measure of interest/penetration

### Control Variables
- Gas prices (regional variation)
- Employment levels (economic activity)
- Average transit fares (pricing effects)
- Service capacity metrics (VRH, VRM, VOMS)
- Population estimates (demographic controls)

### Identification Strategy
We exploit the **staggered rollout** of Uber across metropolitan areas, leveraging:
- **Temporal variation** in market entry timing
- **Cross-sectional variation** across different MSAs
- **Within-agency variation** over time

## 📊 Dataset

### Data Sources
- **Primary**: Hall, Palsson, and Price (2018) dataset
- **Transit Data**: Monthly ridership from U.S. public transit agencies
- **Treatment Data**: Uber market entry dates and Google Trends
- **Controls**: Economic and demographic indicators

### Sample Characteristics
- **Time Period**: 2004-2015 (12 years)
- **Geographic Coverage**: Multiple U.S. Metropolitan Statistical Areas
- **Agencies**: 545 public transit agencies
- **Observations**: 58,379 agency-month observations
- **Balanced Panel**: Comprehensive coverage across time and space

### Data Processing
- Aggregation of duplicate observations
- Missing value handling
- Log transformation of dependent variables
- Panel index construction

## Authors
- Haoyan Liu
- Binghan Zhang
- Xinong Shi
- Sihanyan Liu
