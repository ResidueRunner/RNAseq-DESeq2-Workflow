# 🧬 RNA-Seq Differential Expression Analysis Workflow

## 📌 Project Overview

This repository implements an end-to-end RNA-Seq differential expression analysis workflow based on:

Love MI, Anders S, Kim V, and Huber W (2015).  
RNA-Seq workflow: gene-level exploratory analysis and differential expression.  
F1000Research 4:1070.  
https://doi.org/10.12688/f1000research.7035.1

The workflow demonstrates gene-level exploratory data analysis and differential expression testing using Bioconductor and DESeq2.

---

## 🎯 Objective

- Perform RNA-Seq count-based differential expression analysis
- Explore sample relationships using PCA and clustering
- Identify significantly differentially expressed genes
- Visualize results using heatmaps and volcano plots
- Implement reproducible bioinformatics workflow in Google Colab

---

## 🧪 Dataset

This project uses the `airway` dataset from Bioconductor, which contains RNA-Seq data from airway smooth muscle cells treated with dexamethasone.

Experimental Design:
- 4 human airway smooth muscle cell lines
- Each cell line: treated (trt) vs untreated (untrt)
- Paired experimental design: ~ cell + dex

---

## 🛠 Tools & Packages Used

- R
- Bioconductor
- DESeq2
- airway (example dataset)
- pheatmap
- ggplot2
- RColorBrewer

---

## 🔬 Workflow Steps

### 1️⃣ Load RNA-Seq Count Data
- Import SummarizedExperiment object
- Inspect sample metadata

### 2️⃣ Pre-filtering
- Remove genes with very low counts

### 3️⃣ Differential Expression Analysis
- Estimate size factors
- Estimate dispersion
- Fit generalized linear model
- Perform Wald test

### 4️⃣ Variance Stabilization
- Apply rlog transformation

### 5️⃣ Exploratory Data Analysis
- PCA plot
- Sample-to-sample distance heatmap

### 6️⃣ Visualization
- Volcano plot
- Heatmap clustering

---

## 📊 Results

- PCA shows clustering by treatment and cell line
- Significantly differentially expressed genes identified
- Upregulated and downregulated genes detected at FDR < 0.1

Output Files:
- PCA_plot.png
- heatmap.png
- volcano_plot.png
- DESeq2_results.csv

---

---

## 🚀 How to Run

This workflow was executed using Google Colab with R installed.

Steps:
1. Install R and Bioconductor packages
2. Load airway dataset
3. Run DESeq2 pipeline
4. Generate plots and export results

---

## 📚 Reference

Love MI, Anders S, Kim V, and Huber W (2015).  
RNA-Seq workflow: gene-level exploratory analysis and differential expression.  
F1000Research 4:1070.  
https://doi.org/10.12688/f1000research.7035.1

This article is distributed under the Creative Commons Attribution License (CC BY).

---

## 👨‍💻 Author

Anurag Yadav  
M.Tech Bioinformatics  
Machine Learning & Bioinformatics Enthusiast  

GitHub: https://github.com/ResidueRunner
LinkedIn: www.linkedin.com/in/anurag-yadav-631533159

## 📂 Repository Structure

