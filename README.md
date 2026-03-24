# London PM2.5 Prediction with Graph Neural Networks

**Author**: Cong Lin 
**Date**: March 2026  
**Course**: URBAN5160

## Project Overview

This project applies a Graph Neural Network (GCN) to predict PM2.5 concentrations at Output Area (OA) level in London. The spatial graph is constructed using Queen contiguity with inverse distance edge weights. A Random Forest baseline is used to demonstrate the importance of spatial relationships.

Key steps:
1. **Data Exploration & Cleaning**: Missing values imputed via spatial interpolation (PM2.5) and median (features). Feature selection via correlation and VIF.
2. **Graph Construction**: Queen adjacency graph with inverse distance weights; grid-based spatial train/test split to avoid data leakage.
3. **Dual-Model Training**: GCN with two graph convolution layers vs. Random Forest (no spatial information).
4. **Evaluation & Spatial Interpretation**: Residual maps, prediction maps, and comparison of spatial patterns.
