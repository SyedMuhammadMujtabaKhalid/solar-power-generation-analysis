# Methodology & Architecture

This document outlines the high-level architecture and methodological workflow adopted for the Solar Power Generation Analysis project.

## 1. Project Workflow

The overall workflow from raw data ingestion to visualization.

```mermaid
graph TD
    A[Raw Kaggle Dataset] --> B[Data Loading - Pandas]
    B --> C[Data Cleaning & Preprocessing]
    C --> D[Feature Engineering]
    D --> E[Exploratory Data Analysis]
    E --> F[Data Visualization]
    F --> G[Insights & Reporting]
```

## 2. Data Cleaning Pipeline

The systematic approach used to ensure data quality and integrity before analysis.

```mermaid
flowchart LR
    A([Raw DataFrame]) --> B{Check Nulls}
    B -- Drop Nulls --> C{Check Duplicates}
    C -- Drop Duplicates --> D[Filter Negative Power]
    D --> E[Calculate IQR]
    E --> F[Remove Outliers]
    F --> G[Feature Selection]
    G --> H([Cleaned DataFrame])
```

## 3. Data Analysis Workflow

The steps taken to extract analytical value from the processed data.

```mermaid
graph TD
    A[Cleaned Dataset] --> B[Statistical Summary]
    B --> C[Categorization]
    C --> D[Group By Aggregation]
    D --> E[Sorting & Correlation]
    E --> F[Pattern Recognition]
```

## 4. Visualization Pipeline

The process of translating analytical structures into visual insights.

```mermaid
graph LR
    A[Processed Data] --> B[Matplotlib/Seaborn]
    B --> C[Bar Charts: Cloud Cover]
    B --> D[Line Plots: Radiation Trend]
    B --> E[Box Plots: Temp Variance]
    B --> F[Scatter Plots: Correlations]
    C --> G([Final Rendered Charts])
    D --> G
    E --> G
    F --> G
```
