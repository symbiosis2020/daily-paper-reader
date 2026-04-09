---
title: Analysis of multicellular anatomical structures from spatial omics data using sosta
title_zh: 利用sosta从空间组学数据中分析多细胞解剖结构
authors: "Gunz, S., Crowell, H. L., Robinson, M. D."
date: 2026-04-07
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.13.682065v3.full.pdf"
tags: ["query:profile-1"]
score: 6.0
evidence: 用于分析组织中多细胞解剖结构的空间组学工具
tldr: 本研究针对空间组学技术能保留组织空间背景的特点，指出现有方法多聚焦单细胞排列，而生物功能常源于多细胞结构。为此，作者提出了基于结构的空间组学数据分析方法，专注于直接分析多细胞解剖结构。他们开发了开源Bioconductor包sosta，并通过两个公开数据集演示了该方法的有效性，为社区提供了实用的分析工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-13-682065-v3/fig-001.webp\", \"caption\": \"Fig 1. Structure-based analysis of spatial omics data. a) Spatial arrangements reflect functions across scale, ranging from the subcellular to the organ level. b) An example histopathology image that illustrates diverse multicellular anatomical structures in the transition from healthy intestinal epithelium to premalignant lesions (taken from [10]). c) Spatial omics technologies are used to study biological phenomena across different scales, ranging from subcellular to multicellular, with correlation also present at different scales. d) Illustrated workflow of density-based reconstruction of anatomical structures using a threshold on the point pattern intensity of cell centroids as implemented in the sosta package, followed by the analysis of anatomical structures by quantifying geometric features, or by using anatomical structure information as a reference scale for downstream analysis. Illustrations in a and c were adapted from Servier Medical Art, licensed under CC-BY 4.0.\", \"page\": 3, \"index\": 1, \"width\": 705, \"height\": 497}]"
motivation: 现有分析方法主要关注单细胞的空间排列，而生物功能往往源于多细胞结构，因此需要直接分析多细胞解剖结构的方法。
method: 开发了开源Bioconductor包sosta，用于从空间组学数据中识别和分析多细胞解剖结构。
result: 使用两个公开数据集验证了sosta的有效性，展示了其在分析多细胞结构方面的应用潜力。
conclusion: 该研究通过sosta工具实现了对空间组学数据中多细胞解剖结构的直接分析，为理解组织功能提供了新视角。
---

## 摘要
空间组学技术能够在保留组织内空间背景的同时，对分子特征进行高分辨率、大规模的量化。现有的分析方法主要关注单细胞的空间排列，而生物功能往往产生于多细胞结构。在此，我们引入了基于结构的空间组学数据分析方法，该方法侧重于对多细胞解剖结构的直接分析。我们使用两个公开可用的数据集阐述了此类分析，并提供了sosta——一个开源的Bioconductor软件包，供广大社区使用。

## Abstract
Spatial omics technologies enable high-resolution, large-scale quantification of molecular features while preserving the spatial context within tissues. Existing analysis methods largely focus on spatial arrangements of single cells, whereas biological function often emerges from multicellular arrangements. Here, we introduce structure-based analysis of spatial omics data, which focuses on the direct analysis of multicellular, anatomical structures. We illustrate this type of analysis using two publicly available datasets and provide sosta, an open-source Bioconductor package for broad community use.