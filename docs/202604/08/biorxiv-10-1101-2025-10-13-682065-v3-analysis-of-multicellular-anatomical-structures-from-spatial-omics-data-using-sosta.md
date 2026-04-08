---
title: Analysis of multicellular anatomical structures from spatial omics data using sosta
title_zh: 利用sosta从空间组学数据中分析多细胞解剖结构
authors: "Gunz, S., Crowell, H. L., Robinson, M. D."
date: 2026-04-07
pdf: "https://www.biorxiv.org/content/10.1101/2025.10.13.682065v3.full.pdf"
tags: ["query:profile-1"]
score: 6.0
evidence: 分析空间组学数据中多细胞解剖结构的工具
tldr: 空间组学技术能在保留组织空间背景的前提下，对分子特征进行高分辨率、大规模量化。然而，现有方法主要聚焦于单细胞的空间排列，而生物学功能常源自多细胞结构。为此，本研究引入了基于结构的空间组学数据分析方法，专注于直接分析多细胞的解剖结构。我们利用两个公开数据集展示了此类分析的应用，并提供了名为sosta的开源Bioconductor软件包供社区广泛使用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-10-13-682065-v3/fig-001.webp\", \"caption\": \"Fig 1. Structure-based analysis of spatial omics data. a) Spatial arrangements reflect functions across scale, ranging from the subcellular to the organ level. b) An example histopathology image that illustrates diverse multicellular anatomical structures in the transition from healthy intestinal epithelium to premalignant lesions (taken from [10]). c) Spatial omics technologies are used to study biological phenomena across different scales, ranging from subcellular to multicellular, with correlation also present at different scales. d) Illustrated workflow of density-based reconstruction of anatomical structures using a threshold on the point pattern intensity of cell centroids as implemented in the sosta package, followed by the analysis of anatomical structures by quantifying geometric features, or by using anatomical structure information as a reference scale for downstream analysis. Illustrations in a and c were adapted from Servier Medical Art, licensed under CC-BY 4.0.\", \"page\": 3, \"index\": 1, \"width\": 705, \"height\": 497}]"
motivation: 现有空间组学分析方法主要关注单细胞的空间排列，而生物学功能往往源于多细胞的组合结构，因此需要新的分析视角。
method: 研究团队开发了名为sosta的开源Bioconductor软件包，用于直接分析组织中的多细胞解剖结构。
result: 通过使用两个公开数据集进行案例演示，验证了这种基于结构的分析方法能够有效揭示多细胞组织的功能信息。
conclusion: sosta作为一个开源Bioconductor软件包，旨在促进基于多细胞解剖结构的空间组学分析在社区中的广泛应用。
---

## 摘要
空间组学技术能够在保留组织内空间背景的同时，对分子特征进行高分辨率、大规模的量化。现有的分析方法主要关注单细胞的空间排列，而生物功能往往产生于多细胞结构。在此，我们介绍基于结构的空间组学数据分析方法，该方法侧重于对多细胞解剖结构的直接分析。我们使用两个公开可用的数据集阐述了此类分析，并提供了sosta——一个开源的Bioconductor软件包，供广大社区使用。

## Abstract
Spatial omics technologies enable high-resolution, large-scale quantification of molecular features while preserving the spatial context within tissues. Existing analysis methods largely focus on spatial arrangements of single cells, whereas biological function often emerges from multicellular arrangements. Here, we introduce structure-based analysis of spatial omics data, which focuses on the direct analysis of multicellular, anatomical structures. We illustrate this type of analysis using two publicly available datasets and provide sosta, an open-source Bioconductor package for broad community use.