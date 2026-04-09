---
title: Transcriptome-based cell type assignment for kidney cell culture models
title_zh: 基于转录组的肾组织培养模型的细胞类型鉴定
authors: "Schobert, M., Boehm, S., Borisov, O., Li, Y., Greve, G., Edemir, B., Woodward, O. M., Jung, H. J., Koettgen, M. M., Westermann, L., Schlosser, P., Hutter, F., Kottgen, A., Haug, S."
date: 2026-04-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.30.715265v1.full.pdf"
tags: ["query:profile-1"]
score: 7.0
evidence: 基于转录组的肾脏细胞培养模型（包括足细胞）细胞类型分配方法
tldr: 本研究开发了一种基于转录组的评估方法（CellMatchR网络工具及TabPFN脚本），用于系统评估肾脏细胞系与原代细胞的相似性。该方法整合了批量RNA-seq数据和单细胞RNA-seq参考数据集，利用统计相关性及机器学习进行匹配验证。研究发现Spearman相关性和TabPFN模型最为准确有效，并应用此方法揭示了常用肾小管细胞系的身份异质性及集合管细胞的稳定性。该工作为肾脏研究提供了选择、解释和质控体外模型的实用资源与方法框架。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-001.webp\", \"caption\": \"Table 1: Matching results for tubular cell lines\", \"page\": 15, \"index\": 1, \"width\": 1077, \"height\": 800}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-002.webp\", \"caption\": \"Figure 3: Matching results for microdissected tubular segments\", \"page\": 14, \"index\": 2, \"width\": 950, \"height\": 842}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-003.webp\", \"caption\": \"Figure 2: Evaluation of matching methods\", \"page\": 13, \"index\": 3, \"width\": 948, \"height\": 1135}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-004.webp\", \"caption\": \"Figure 1: Study workflow\", \"page\": 12, \"index\": 4, \"width\": 950, \"height\": 477}]"
motivation: 肾脏细胞系是研究肾脏生理和疾病的重要工具，但其基因表达谱可能因永生化、培养条件或实验处理而与原代细胞不同，因此需要一种系统方法来评估其与原代细胞的相似性。
method: 开发了一种基于转录组的方法，通过将细胞系或组织的批量RNA-seq数据与来自单细胞RNA-seq数据集的参考细胞类型进行匹配，使用了三种统计相似性度量和三种机器学习分类器进行评估。
result: 基于基因表达排名的Spearman相关性和表格数据基础模型TabPFN被证明是最准确和特异的方法；应用该方法发现常用肾小管细胞系的身份匹配情况不一，而集合管来源的mIMCD-3细胞则表现稳定。
conclusion: 本研究为肾脏研究领域提供了一个实用的资源和方法框架，有助于研究人员基于转录组相似性，为体外实验知情地选择细胞模型、进行质量控制，并更可靠地将体外发现转化应用于肾脏生理和疾病研究。
---

## 摘要
背景
肾脏细胞系被广泛用于模拟肾脏生理和疾病；然而，由于永生化、培养条件或实验处理，其基因表达谱可能与原代细胞存在差异。确定一个细胞系是否与其天然细胞类型相似，对于解释体外研究结果至关重要。我们开发了一种基于转录组的方法，将来自肾脏细胞系、原代细胞或组织的批量RNA-seq数据与源自单细胞RNA-seq（scRNA-seq）数据集的参考细胞类型进行匹配。

方法
通过伪批量聚合，从两个人类和两个小鼠肾脏scRNA-seq数据集生成参考转录组谱。使用三种统计相似性度量（斯皮尔曼相关性、欧几里得距离、泊松距离）和三种机器学习分类器（随机森林、XGBoost、TabPFN），将来自显微切割肾组织、非肾脏阴性对照以及肾脏细胞系的批量RNA-seq数据与这些参考谱进行匹配。每种方法均使用全局基因表达、精选的肾脏标志基因列表以及变异最大的基因进行评估。通过三步验证策略评估匹配准确性：数据集内匹配、跨参考比较以及对原代肾组织和阴性对照的验证。

结果
基于基因表达排序的斯皮尔曼相关性和TabPFN（一种用于表格数据的基础模型）成为最准确和特异性的方法，尤其是在使用精选的肾脏标志基因列表时。两种方法均能正确识别显微切割的肾小管节段，并且对非肾脏阴性对照具有稳健性。应用于常用的肾脏细胞系时，OK细胞保留了近端小管特性，尤其是在剪切应力条件下；而其他近端小管来源的细胞系（HK-2, HKC-8, HKC-11）则显示出不一致的匹配结果。集合管来源的mIMCD-3在不同传代次数、培养条件和遗传修饰下均保持稳定的相似性。

结论
我们提供了两种互补的实现方式：CellMatchR——一个易于使用的基于网络的工具，利用斯皮尔曼相关性进行常规分析；以及用于基于TabPFN匹配的综合脚本（链接将在同行评审发表后添加）。这些资源共同使研究人员能够就肾脏细胞培养模型的选择、解释和稳定性做出明智决策。

转化声明
肾脏细胞系是肾病学研究的基本工具，但其与天然细胞类型的转录组相似性很少得到系统验证。我们证明，将批量RNA-seq数据与单细胞参考数据集相结合，能够利用基于基因表达排序的相关性和机器学习方法对细胞系身份进行稳健评估。通过对匹配方法、精选的肾脏标志基因列表和参考数据集进行全面评估，我们的研究既可作为肾病学界的实用资源，也可作为方法论框架，有助于知情选择细胞培养模型、实验条件的质量控制、开发新的实验性细胞培养模型以及更可靠地将体外研究发现转化应用于理解肾脏生理和疾病。

## Abstract
BackgroundKidney cell lines are widely used to model kidney physiology and disease; however, their gene expression profiles may differ from primary cells due to immortalization, culture conditions, or experimental treatments. Determining whether a cell line resembles its native cell type is critical for interpreting in vitro findings. We developed a transcriptome-based approach that matches bulk RNA-seq data from kidney cell lines, primary cells, or tissues to reference cell types derived from single-cell RNA-seq (scRNA-seq) datasets.

MethodsReference transcriptomic profiles were generated from two human and two murine kidney scRNA-seq datasets by pseudobulk aggregation. Bulk RNA-seq data from microdissected kidney tissue, non-kidney negative controls, and kidney cell lines were matched to these references using three statistical similarity measures (Spearman correlation, Euclidean distance, Poisson distance) and three machine learning classifiers (Random Forest, XGBoost, TabPFN). Each was assessed with global gene expression, curated kidney marker gene lists, and the most variable genes. Matching accuracy was evaluated through a three-step validation strategy: within-dataset matching, cross-reference comparison, and validation against primary kidney tissue and negative controls.

ResultsGene expression rank-based Spearman correlation and TabPFN, a foundation model for tabular data, emerged as the most accurate and specific approaches, particularly with curated kidney marker gene lists. Both methods correctly identified microdissected kidney tubule segments and were robust against non-kidney negative controls. Applied to commonly used kidney cell lines, OK cells retained proximal tubule identity, particularly under shear stress, while other proximal tubule lines (HK-2, HKC-8, HKC-11) showed inconsistent matching. Collecting duct-derived mIMCD-3 maintained stable similarity across passages, culture conditions, and genetic modifications.

ConclusionWe provide two complementary implementations: CellMatchR, an accessible web-based tool using Spearman correlation for routine use, and comprehensive scripts for TabPFN-based matching (link will be added after peer reviewed publication). Together, these resources enable researchers to make informed decisions about kidney cell culture model selection, interpretation, and stability.

Translational StatementKidney cell lines are fundamental tools in nephrology research, yet their transcriptomic similarity to native cell types is rarely validated systematically. We demonstrate that combining bulk RNA-seq data with single-cell reference datasets enables robust assessment of cell line identity using gene expression-rank-based correlation and machine learning approaches. By providing a comprehensive evaluation of matching methods, curated kidney marker gene lists, and reference datasets, our study serves as both a practical resource and a methodological framework for the kidney research community, facilitating informed selection of cell culture models, quality control of experimental conditions, developing new experimental cell culture models, and more reliable translation of in vitro findings to kidney physiology and disease.