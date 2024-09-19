# Laplacian of a Graph and Applications in Mapping AI and Common Stocks Relationships
This project explores the application of the Laplacian matrix in analyzing relationships between AI stocks and other stocks in the stock market. It uses graph-based techniques to model these relationships, helping identify clusters, central stocks, and the role of AI stocks within the broader market.

## Table of Contents
Introduction
Project Structure
Installation
Usage
Data
Experiments and Results
Conclusion
Future Work
References
Introduction
This project focuses on using the Laplacian matrix to study the relationships between AI-related stocks (such as NVIDIA) and other sectors. By constructing graphs with stocks as nodes and their relationships based on stock performance as edges, we can analyze the market structure, identify stock clusters, and discover central stocks that play key roles in market dynamics.

## Key Concepts:
Laplacian Matrix: Used to model graph structure.
Fiedler Value: Helps in identifying stock market connectivity and clustering.
Graph Neural Networks (GNNs): Used to model non-linear relationships between stocks.
Project Structure
The repository contains the following files:

CSV Files: Financial data for various sectors, including AI, banking, biotechnology, and manufacturing.
AI_financial_data.csv
Banking_financial_data.csv
Biotechnology_financial_data.csv
Manufacturing_financial_data.csv
Technology_financial_data.csv
combined_financial_data.csv (Aggregated data from all sectors)
Jupyter Notebooks: Code for data preprocessing, graph construction, and experimentation.
Main_code.ipynb: Main analysis script.
Crawl_data.ipynb: Used for collecting and preparing data.
Images (PNG): Visualizations of graphs and results.
fig1.png, fig2.png, fig3.png, fig4.png: Graph plots showing stock relationships.
Word Document: Term paper explaining the theory and methodology.
term_paper.docx

## Installation
To run this project, ensure you have the following dependencies installed:

bash
Copy code
pip install pandas numpy matplotlib networkx jupyter
Alternatively, use the requirements.txt file to install the necessary packages:

bash
Copy code
pip install -r requirements.txt
Usage
Step 1: Data Preprocessing
Run Crawl_data.ipynb to collect and preprocess the stock data.
The data files are provided in CSV format and contain financial information such as stock prices, P/E ratios, and Beta values.
Step 2: Graph Construction and Laplacian Matrix Calculation
Open Main_code.ipynb to construct the graph of stocks based on their relationships (correlations).
The Laplacian matrix is computed to analyze the graph, identify clusters, and visualize connections between stocks.

Step 3: Visualization

Visualizing stock relationships.

Data
The dataset includes stock price and financial information for various sectors from 2018 to June 2024.

Key columns:

Stock Prices
P/E Ratio
Beta
P/B Ratio

The data is grouped by sectors:

AI (NVIDIA, etc.)
Semiconductors
Biotechnology
Energy and Electric
Manufacturing
Banking
Gaming
Experiments and Results
Key insights include:

NVIDIA and other major tech stocks (MSFT, GOOGL, AMZN) form strong clusters, indicating high correlation within the technology sector.
The Laplacian matrix eigenvalues help identify weaker relationships between sectors like biotechnology and gaming.
The results are visualized in fig1.png, fig2.png, and other related images, showing stock clustering and connectivity.

## Conclusion
This project successfully demonstrates how the Laplacian matrix can be used to model stock market relationships. It highlights the central role of AI stocks like NVIDIA within the stock network and shows how graph-based analysis can provide meaningful insights for investors.

## Future Work
Future work will include expanding the dataset and applying more advanced models such as Deep Canonical Correlation Analysis (DCCA) to further improve the analysis of stock market relationships. Additionally, integration with Large Language Models (LLM) to enrich financial datasets is planned.

## References
M. Fiedler, “Algebraic connectivity of graphs.”
D. A. Spielman and S.-H. Teng, “Spectral partitioning works.”
Papers related to non-linearity in Graph Neural Networks.
