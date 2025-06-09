# ClusteredAnalysis

Company Segmentation with K-Means Variants
Asia Business Performance Case Study
Exploring clustering algorithms to segment companies based on financial performance—through the lens of ethical, interpretable, and policy-relevant data science.

## Overview
This project analyzes the Asia Magazine business dataset using multiple clustering techniques to segment companies by financial performance indicators such as revenue, profit, assets, and market capitalization.
The goal was to compare different unsupervised learning methods, evaluate their interpretability, and assess how segmentation structures vary with changes in algorithmic, statistical, and distance-based parameters.

## Business and Policy Motivation
Company segmentation is a foundational step in strategic planning—whether for venture capital targeting, macroeconomic policy differentiation, or SME development programs. Yet, segmentation methods often overlook transparency, bias, and interpretability.

This project attempts to:
Uncover meaningful clusters in firm performance
Highlight how different methodological choices (e.g., normalization or distance metric) impact outcomes
Reflect on the interpretive responsibility of data scientists when designing unsupervised systems

## Techniques & Methodologies
Data Preprocessing
Iterative imputation of missing values using tree-based methods
Normalization via Min-Max scaling and Z-score standardization
Clustering Algorithms
Lloyd's k-means
Elkan’s k-means
MacQueen’s k-means

## Evaluation Metrics
Cosine similarity between segmentation outputs
Normalized mean plots of cluster centers
Variable importance scores
Outlier detection via small cluster analysis

## Selected Models
Label	Algorithm	Init	Distance	Norm.	Clusters
EKEZ_2	Elkan	k-means++	Euclidean	Z-score	2
MRMR_4	MacQueen	Random	Manhattan	Range	4
LREZ_E	Lloyd	Random	Euclidean	Z-score	Elbow-determined
The EKEZ_2 model most effectively distinguished high-cap, high-revenue companies from emerging firms, with strong separation across profitability and asset metrics.

## Key Insights
Choice of normalization significantly affects cluster structures.
Elkan’s method with Euclidean distance produced the most interpretable segmentation.
An outlier cluster (n=14) in LREZ_E may represent a niche market or data anomaly requiring expert validation.
Cosine similarity analysis showed that MRMR_4 and LKER_E were structurally similar, while EKEZ_2 was distinct.

## Ethical Reflection
Clustering is often treated as objective, but it reflects assumptions—about scaling, distance, and what matters most. In this project, variable importance tracking, outlier handling, and interpretability were prioritized to ensure the outputs could meaningfully support inclusive, accountable decision-making in contexts like economic planning or social entrepreneurship support.
