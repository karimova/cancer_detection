# Early Cancer Detection
<img src="p-4.jpg" alt="cancer" width="600">

## Problem Statement

The Indian Council of Medical Research (ICMR) is dedicated to studying the underlying causes of different types of cancers, such as breast cancer, renal cancer, colon cancer, lung cancer, and prostate cancer. These types of cancer have emerged as significant concerns in recent years. The primary goal is to identify the specific genetic factors that contribute to each type of cancer, allowing for early detection and intervention. By uncovering these genetic markers, the aim is to reduce the fatality rate associated with these cancers and improve patient outcomes.

## Dataset Details

The dataset consists of 802 samples from individuals diagnosed with different types of cancer. Each sample contains the expression values of more than 20,000 genes. The samples are categorized into the following types of tumors: BRCA, KIRC, COAD, LUAD, and PRAD.

## Steps

### Step 1: Exploratory Data Analysis

- Merge the datasets.
- Visualize the merged dataset as a hierarchically-clustered heatmap.
- Perform null-hypothesis testing.

### Step 2: Dimensionality Reduction

Given a large number of genes (20,000+) in each sample, it is not necessary to include all gene expression values for analyzing each cancer type. The goal is to identify a smaller set of informative attributes for fitting multiclass classification models. Dimensionality reduction techniques such as PCA, LDA, and t-SNE will be employed.

### Step 3: Clustering Genes and Samples

The objective is to identify groups of genes that exhibit similar behavior across samples and examine the distribution of samples corresponding to each cancer type. Various clustering techniques, including k-means, hierarchical, and mean-shift clustering, will be applied to genes and samples.

- Identify genes with similar expression values across all samples.
- Identify samples belonging to the same cancer type and cluster.

### Step 4: Building Classification Model(s) with Feature Selection

The final task involves constructing robust classification models to identify each type of cancer.

- Build classification models using multiclass SVM, Random Forest, and Deep Neural Network.
- Apply feature selection algorithms (forward selection and backward elimination) using the selected attributes from Step 2.
- Validate the selected genes using statistical significance testing (F-test).

By completing these steps, I aim to contribute to early cancer detection by developing effective classification models that can accurately identify different types of cancer based on genetic attributes.
