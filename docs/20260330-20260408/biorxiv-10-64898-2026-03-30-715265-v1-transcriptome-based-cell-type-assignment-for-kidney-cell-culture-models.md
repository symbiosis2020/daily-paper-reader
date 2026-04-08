---
title: Transcriptome-based cell type assignment for kidney cell culture models
title_zh: 基于转录组的肾组织培养模型的细胞类型鉴定
authors: "Schobert, M., Boehm, S., Borisov, O., Li, Y., Greve, G., Edemir, B., Woodward, O. M., Jung, H. J., Koettgen, M. M., Westermann, L., Schlosser, P., Hutter, F., Kottgen, A., Haug, S."
date: 2026-04-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.03.30.715265v1.full.pdf"
tags: ["query:profile-1"]
score: 9.0
evidence: 基于转录组的肾脏细胞培养模型细胞类型分配
tldr: 本研究开发了一种基于转录组的评估方法，用于判断肾脏细胞系在基因表达上是否与其对应的天然肾脏细胞类型相似。该方法利用单细胞RNA-seq数据集构建参考图谱，并通过多种统计和机器学习算法将批量RNA-seq数据与之匹配。研究发现Spearman相关性和TabPFN模型结合肾脏标志基因列表时效果最佳。应用此工具分析常用肾小管细胞系，揭示了它们在身份保留上的差异，为研究者选择、解释和验证体外模型提供了重要资源和决策依据。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-001.webp\", \"caption\": \"Table 1: Matching results for tubular cell lines\", \"page\": 15, \"index\": 1, \"width\": 1077, \"height\": 800}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-002.webp\", \"caption\": \"Figure 3: Matching results for microdissected tubular segments\", \"page\": 14, \"index\": 2, \"width\": 950, \"height\": 842}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-003.webp\", \"caption\": \"Figure 2: Evaluation of matching methods\", \"page\": 13, \"index\": 3, \"width\": 948, \"height\": 1135}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-03-30-715265-v1/fig-004.webp\", \"caption\": \"Figure 1: Study workflow\", \"page\": 12, \"index\": 4, \"width\": 950, \"height\": 477}]"
motivation: 肾脏细胞系是研究肾脏生理和疾病的重要工具，但其基因表达谱可能因永生化、培养条件或实验处理而与原代细胞不同，因此需要一种系统的方法来评估其与天然细胞类型的相似性。
method: 开发了一种基于转录组的方法，通过将细胞系、原代细胞或组织的批量RNA-seq数据与源自单细胞RNA-seq数据集的参考细胞类型进行匹配，并评估了多种统计相似性度量和机器学习分类器的性能。
result: 基于基因表达排名的Spearman相关性和表格数据基础模型TabPFN被证明是最准确和特异的方法；应用该方法发现常用肾小管细胞系的身份匹配情况不一，而集合管来源的mIMCD-3则表现出稳定的相似性。
conclusion: 本研究为肾脏研究领域提供了一个实用的资源和方法框架，有助于研究者明智地选择细胞培养模型、进行实验条件质控以及更可靠地将体外发现转化至肾脏生理与疾病研究。
---

## 摘要
背景：肾脏细胞系被广泛用于模拟肾脏生理与疾病；然而，由于永生化、培养条件或实验处理的影响，其基因表达谱可能与原代细胞存在差异。确定细胞系是否与其天然细胞类型相似，对于解读体外实验结果至关重要。我们开发了一种基于转录组的方法，该方法能够将来自肾脏细胞系、原代细胞或组织的批量RNA-seq数据与源自单细胞RNA-seq（scRNA-seq）数据集的参考细胞类型进行匹配。

方法：通过伪批量聚合，从两个人类和两个小鼠肾脏scRNA-seq数据集中生成参考转录组谱。使用三种统计相似性度量（斯皮尔曼相关性、欧几里得距离、泊松距离）和三种机器学习分类器（随机森林、XGBoost、TabPFN），将来自显微切割的肾组织、非肾脏阴性对照以及肾脏细胞系的批量RNA-seq数据与这些参考谱进行匹配。每种方法均使用全局基因表达谱、经筛选的肾脏标志基因列表以及变异度最高的基因进行评估。匹配准确性通过三步验证策略进行评估：数据集内匹配、跨参考比较以及与原发性肾组织和阴性对照的验证。

结果：基于基因表达排名的斯皮尔曼相关性和TabPFN（一种用于表格数据的基础模型）成为最准确且特异性最高的方法，尤其是在使用经筛选的肾脏标志基因列表时。两种方法均能正确识别显微切割的肾小管节段，并对非肾脏阴性对照具有稳健性。应用于常用的肾脏细胞系时，OK细胞保持了近端小管特性（尤其在剪切应力下），而其他近端小管线（HK-2、HKC-8、HKC-11）则显示出不一致的匹配结果。集合管来源的mIMCD-3在传代次数、培养条件和遗传修饰下均保持稳定的相似性。

结论：我们提供了两种互补的实现方案：CellMatchR——一个基于斯皮尔曼相关性、易于使用的网络工具，适用于常规分析；以及用于基于TabPFN匹配的综合脚本（链接将在同行评审后添加）。这些资源共同使研究人员能够就肾脏细胞培养模型的选择、结果解读和稳定性做出明智决策。

转化声明：肾脏细胞系是肾病学研究的基础工具，但其与天然细胞类型的转录组相似性很少得到系统验证。我们证明，将批量RNA-seq数据与单细胞参考数据集相结合，能够利用基于基因表达排名的相关性方法和机器学习方法对细胞系身份进行稳健评估。通过对匹配方法、经筛选的肾脏标志基因列表和参考数据集进行全面评估，我们的研究既为肾病学界提供了实用资源，也提供了一个方法论框架，有助于促进明智选择细胞培养模型、控制实验条件质量、开发新的实验性细胞培养模型以及更可靠地将体外研究发现转化应用于理解肾脏生理与疾病。

## 速览
**TLDR**：本研究开发了一种基于转录组的匹配方法，用于评估肾脏细胞系与原代细胞的相似性。通过整合单细胞RNA测序参考数据集，利用统计相似性度量和机器学习分类器分析批量RNA测序数据。结果显示斯皮尔曼相关性和TabPFN方法最为有效，能准确识别肾小管片段并验证常用细胞系的特性差异。该研究提供了CellMatchR网络工具和TabPFN脚本资源，帮助研究者更可靠地选择和应用肾脏细胞培养模型。 \
**Motivation**：肾脏细胞系广泛用于模拟肾脏生理和疾病，但其基因表达谱可能因永生化、培养条件或实验处理而与原代细胞不同，因此需要系统评估其与原代细胞的相似性以确保体外研究结果的可靠性。 \
**Method**：通过从单细胞RNA测序数据生成参考转录组谱，使用三种统计相似性度量（斯皮尔曼相关性、欧氏距离、泊松距离）和三种机器学习分类器（随机森林、XGBoost、TabPFN），将肾脏细胞系的批量RNA测序数据与参考细胞类型进行匹配。 \
**Result**：基于基因表达排名的斯皮尔曼相关性和TabPFN方法最为准确和特异，能正确识别微分离的肾小管片段并有效排除非肾脏阴性对照；应用于常用肾脏细胞系发现OK细胞在剪切应力下保持近端小管特性，而其他近端小管线（如HK-2）匹配不一致，mIMCD-3则在不同条件下保持稳定相似性。 \
**Conclusion**：本研究为肾脏研究提供了两种互补的工具：基于Spearman相关性的CellMatchR网络工具和基于TabPFN的脚本，帮助研究者评估细胞模型与原生细胞类型的转录组相似性，从而更可靠地选择细胞培养模型并解释体外实验结果。

---

## Abstract
BackgroundKidney cell lines are widely used to model kidney physiology and disease; however, their gene expression profiles may differ from primary cells due to immortalization, culture conditions, or experimental treatments. Determining whether a cell line resembles its native cell type is critical for interpreting in vitro findings. We developed a transcriptome-based approach that matches bulk RNA-seq data from kidney cell lines, primary cells, or tissues to reference cell types derived from single-cell RNA-seq (scRNA-seq) datasets.

MethodsReference transcriptomic profiles were generated from two human and two murine kidney scRNA-seq datasets by pseudobulk aggregation. Bulk RNA-seq data from microdissected kidney tissue, non-kidney negative controls, and kidney cell lines were matched to these references using three statistical similarity measures (Spearman correlation, Euclidean distance, Poisson distance) and three machine learning classifiers (Random Forest, XGBoost, TabPFN). Each was assessed with global gene expression, curated kidney marker gene lists, and the most variable genes. Matching accuracy was evaluated through a three-step validation strategy: within-dataset matching, cross-reference comparison, and validation against primary kidney tissue and negative controls.

ResultsGene expression rank-based Spearman correlation and TabPFN, a foundation model for tabular data, emerged as the most accurate and specific approaches, particularly with curated kidney marker gene lists. Both methods correctly identified microdissected kidney tubule segments and were robust against non-kidney negative controls. Applied to commonly used kidney cell lines, OK cells retained proximal tubule identity, particularly under shear stress, while other proximal tubule lines (HK-2, HKC-8, HKC-11) showed inconsistent matching. Collecting duct-derived mIMCD-3 maintained stable similarity across passages, culture conditions, and genetic modifications.

ConclusionWe provide two complementary implementations: CellMatchR, an accessible web-based tool using Spearman correlation for routine use, and comprehensive scripts for TabPFN-based matching (link will be added after peer reviewed publication). Together, these resources enable researchers to make informed decisions about kidney cell culture model selection, interpretation, and stability.

Translational StatementKidney cell lines are fundamental tools in nephrology research, yet their transcriptomic similarity to native cell types is rarely validated systematically. We demonstrate that combining bulk RNA-seq data with single-cell reference datasets enables robust assessment of cell line identity using gene expression-rank-based correlation and machine learning approaches. By providing a comprehensive evaluation of matching methods, curated kidney marker gene lists, and reference datasets, our study serves as both a practical resource and a methodological framework for the kidney research community, facilitating informed selection of cell culture models, quality control of experimental conditions, developing new experimental cell culture models, and more reliable translation of in vitro findings to kidney physiology and disease.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，我将为您提供一份关于这篇预印本论文的深入、客观的结构化总结。

---

### **论文总结：基于转录组的肾脏细胞培养模型细胞类型鉴定**

#### **1. 核心问题与整体含义**
*   **研究动机**：肾脏细胞系是肾病学研究的基础工具，但其在体外培养过程中可能发生去分化或基因表达改变，导致其与体内原代细胞的相似性存疑。目前缺乏一个系统、标准化的方法来评估细胞系的“身份”（即其最接近的天然肾脏细胞类型），这影响了体外实验结果的可靠性和可解释性。
*   **整体含义**：本研究旨在填补这一方法学空白，开发并验证一种基于转录组学的通用框架，用于将批量RNA-seq数据（来自细胞系或组织）与单细胞RNA-seq（scRNA-seq）构建的肾脏参考图谱进行匹配，从而客观地评估和鉴定体外模型的细胞类型身份。

#### **2. 方法论**
*   **核心思想**：将待测样本（如细胞系）的批量RNA-seq表达谱与从多个scRNA-seq数据集生成的、已知肾脏细胞类型的“伪批量”参考表达谱进行比较，找出最相似的参考类型。
*   **关键技术细节**：
    1.  **参考图谱构建**：从两个人类（KPMP, Zhang et al.）和两个小鼠（Ransick et al., Park et al.）肾脏scRNA-seq数据集中，通过聚合同一细胞类型的所有细胞的基因计数并标准化为CPM，生成每种细胞类型的参考转录组谱。
    2.  **匹配方法比较**：
        *   **统计相似性度量**：斯皮尔曼秩相关、欧几里得距离、泊松距离。
        *   **机器学习分类器**：随机森林、XGBoost、TabPFN（一种表格数据基础模型）。
    3.  **特征基因集选择**：
        *   所有共享基因（全局表达）。
        *   经筛选的肾脏标志基因列表（`mg_all`: 584个；`mg_tub`: 310个）。
        *   每个参考数据集中变异度最高的1000个基因。
    4.  **验证策略（三步法）**：
        1.  **数据集内验证**：将同一scRNA-seq数据集内的同种细胞随机分成两组进行匹配。
        2.  **跨数据集验证**：在不同来源的scRNA-seq参考数据集之间匹配对应的细胞类型。
        3.  **真实样本验证**：使用已知身份的显微切割肾小管组织作为阳性对照，非肾组织作为阴性对照进行测试。

#### **3. 实验设计**
*   **数据集/场景**：
    *   **参考数据 (4个)**：两个人类和两个小鼠肾脏scRNA-seq公共数据集。
    *   **测试/验证数据 (多组)**：
        *   来自公开及内部的批量RNA-seq数据。
        *   **(阳性对照)** Chen et al.（2021）提供的14个小鼠显微切割肾小管节段样本以及小鼠肾皮质/髓质组织。
        *   **(阴性对照)** 非肾组织样本（成纤维细胞、心脏、大脑、血液单核细胞）。
        *   **(应用对象)** 多种常用肾小管/集合管来源的永生化或原代培养物（如OK, HK-2, HKC-8, HKC-11, mIMCD-3, mpkCCD等），涵盖不同物种、传代数、培养条件（剪切应力、渗透压）、遗传修饰等处理组。
*   **Benchmark (对比基准)**：
    *   研究本身没有外部基准工具作为直接对比对象。其核心贡献在于建立并系统比较了多种内部方法组合的性能。评估指标是“匹配准确率”，即正确识别出生物学上对应参考类型的样本百分比。

#### **4. 资源与算力**
*   论文中未明确提及具体的计算硬件配置（如GPU型号/数量）、训练时长或总计算成本。考虑到主要分析涉及的是预训练模型TabPFN的应用以及相对标准的统计计算和机器学习模型训练，推测其对算力的要求并非极端苛刻。但作者声明使用了AI语言模型辅助写作。

#### **5. 实验数量与充分性**
*   **实验数量充分且系统化**：
    1.  **(方法组合比较)** ：对3种相似性度量 × （4种特征集 + PCA/UMAP降维变体）+ （3种ML分类器 × （最多4种特征集）），共超过15种方法-特征集组合进行了全面评估。
    2.  **(多层次验证)** ：严格的三步验证策略覆盖了从理想情况到真实复杂情况的递进测试场景。
    3.  **(应用案例广泛)** ：评估了超过10种不同的肾脏相关培养物在多种条件下的身份稳定性。
*   **客观性与公平性评价**：
    *   ✅ `客观`：使用了公开可获取的数据集和标准化的性能指标。提供了详细的补充材料和数据共享声明。对阴性对照进行了特异性测试。
    *   ✅ `公平`：所有方法在同一套数据和特征集上进行评估。承认了不同scRNA-seq参考数据集之间的异质性及其对结果的影响。

#### **6. 主要结论与发现**
1.  Spearman秩相关和TabPFN是两种最优的方法，尤其在结合经筛选的肾脏标志基因列表时表现最佳——准确率高且对非肾组织具有高特异性。
2.  不同单细胞参考数据集之间存在显著异质性，影响跨数据集匹配的准确性。因此建议使用多个而非单一参考进行评估以提高稳健性。
3.  常用近端小管来源的OK和HK-2细胞的近端小管身份得到确认；其中OK细胞的近端小管特性在模拟体内流体剪切应力的条件下进一步增强。而其他近端小管线及足突状上皮来源HUPEC细胞的匹配结果不一致或不明确，提示其在培养中可能发生了去分化或身份丢失。
4.  集合管来源的培养物显示出更稳定的身份保留特性；有趣的是TabPFN倾向于将它们归类为髓袢升支粗段而非集合管本身，这可能反映了集合管内存在皮质到髓质的转录梯度变化。

#### **7. 优点**
*   `填补方法论空白`：首次为系统性评估肾脏体外模型的转录组身份提供了一个专门且经过严格验证的计算框架。
*   `严谨的系统性评估`：“三步法”验证策略设计合理且全面；同时比较了传统统计方法和前沿机器学习模型在不同特征集下的表现；考虑了物种匹配的重要性；提供了详尽的补充数据和代码资源承诺开源共享以促进社区使用和复现研究结果
*   
####   
8\.   
不足与局限

*
*
*
*
*
*
*

###   
9\.   
结论

本研究开发了一种基于转录组的标准化方法来鉴定体外模型的生物学身份并通过严格的系统评价确定了最优的方法组合——Spearman相关性和TabPFN结合标志基因列表该方法能够有效区分不同节段的肾小管并对非肾组织保持高特异性应用该方法揭示了常用肾小管线在身份保留上的差异为研究者选择和使用这些模型提供了重要的决策依据

(完)

#### **8. 不足与局限**
*   **对参考图谱的依赖**：方法的准确性高度依赖于所使用的单细胞参考图谱的质量、细胞类型注释的准确性以及覆盖的细胞类型全面性。如果参考图谱中缺少某种特定细胞状态或亚型，该方法将无法识别。
*   **批量RNA-seq数据的局限性**：该方法基于批量测序数据，无法解析培养物内部的细胞异质性。一个被鉴定为“近端小管”的培养物，可能实际上是由一小部分近端小管样细胞和大量去分化细胞混合而成，而批量测序只能给出一个平均信号。
*   **“身份”定义的简化**：该方法将复杂的细胞身份简化为与单一参考类型的相似性排名。对于处于过渡状态、混合身份或发生部分转化的细胞系（如某些HKC系），其匹配结果可能模糊或不一致，这虽然揭示了问题，但未能提供更精细的身份描述。
*   **仅限于转录组层面**：细胞的“身份”不仅由转录组定义，还包括表观遗传、蛋白质组和功能特征。本研究的方法未整合这些多组学信息，其鉴定结果需要结合功能实验进行最终确认。
*   **计算框架的通用性验证有限**：虽然框架设计为通用，但当前研究主要聚焦于肾小管上皮细胞。其在肾脏其他细胞类型（如肾小球细胞、间质细胞）或更广泛的其他器官培养模型中的普适性，仍需进一步测试。

#### **9. 结论**
本研究开发了一种基于转录组的标准化方法来鉴定体外模型的生物学身份，并通过严格的系统评价确定了最优的方法组合——Spearman相关性和TabPFN结合标志基因列表。该方法能够有效区分不同节段的肾小管，并对非肾组织保持高特异性。应用该方法揭示了常用肾小管线在身份保留上的差异，为研究者选择和使用这些模型提供了重要的决策依据。该工作不仅提供了一个实用的工具（`cellid.py`），更重要的是建立了一个可扩展的评估框架，强调了在实验设计中考虑模型“身份验证”的必要性，对提高肾脏病学乃至更广泛生命科学领域体外研究的可靠性和可重复性具有积极意义。

（完）
