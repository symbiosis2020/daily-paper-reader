---
title: A population-scale atlas of blood and tissue in lupus nephritis
title_zh: 狼疮性肾炎的血液与组织群体规模图谱
authors: "Sugiarto, N. W., Gurajala, S., Curtis, M., Eisenhaure, T. M., Arazi, A., Fava, A., Xiao, Q., Mears, J., Rovin, B., Berthier, C. C., Zhao, Y., Izmirly, P. M., Barnas, J. L., Hoover, P. J., Peters, M., Raychowdhury, R., Horisberger, A., Sakaue, S., Furie, R. A., Belmont, H. M., Hildeman, D. A., Woodle, E. S., Dall'Era, M., Putterman, C., Kamen, D. L., McMahon, M. A., Grossman, J., Kalunian, K. C., Hodgin, J. B., Payan-Schober, F., Apruzzese, W., Perlman, H., Cuda, C. M., Wofsy, D., Guthridge, J. M., Anolik, J. H., James, J. A., Accelerating Medicines Partnerships Rheumatoid Arthritis/Systemic Lu"
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.1101/2025.08.11.669754v3.full.pdf"
tags: ["query:q6"]
score: 8.0
evidence: 狼疮性肾炎单细胞图谱，识别肾组织中的免疫群体
tldr: 本研究构建了狼疮性肾炎（LN）患者血液和肾脏组织的单细胞图谱，通过对155名患者和30名对照的样本进行大规模单细胞测序分析，揭示了肾脏组织内的基质和免疫细胞群体。研究发现疤痕相关巨噬细胞（SAMs）与肾脏疾病活动性相关，并在活动性疾病中更多地浸润肾小球，可能驱动肾纤维化。这表明靶向髓系细胞群或可成为预防LN肾脏炎症和损伤的新治疗策略。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-001.webp\", \"caption\": \"Fig. 4. Case-control associations within cell types. A-G CNA results for case-control association with no covariate corrections, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with LN, with FDR cutoff of 0.05. Blue and red denote contracted and expanded neighborhoods that pass\", \"page\": 58, \"index\": 1, \"width\": 979, \"height\": 1147}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-002.webp\", \"caption\": \"Fig. 6. Cell states associated with activity index. (A), Across all cell types, CNA results for activity index association while adjusting for first biopsy, site, and chronicity index, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with activity index, with FDR cutoff of 0.1. Dashed vertical lines represent the correlation threshold with FDR < 0.1. Non-significant associations are colored in grey. P-value is the global P-value for cell state associations with activity index phenotype. Right - violin plots of clusters containing cells passing FDR significance for activity index association. (B), Same\", \"page\": 62, \"index\": 2, \"width\": 979, \"height\": 1020}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-003.webp\", \"caption\": \"Fig. 5. Cell states associated with chronicity index. (A), Univariate CNA of each cell type testing for relevant clinical and demographic variables. * indicates a global p-value < 0.05. (B), For each cell\", \"page\": 60, \"index\": 3, \"width\": 979, \"height\": 1099}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-004.webp\", \"caption\": \"Fig. 2. Cell state annotations in tissue. (A) UMAP of T/NK cell states in tissue, colored by fine grain cell state annotations. Annotation boxes are located at the centroid (mean) of each cluster. (B-H), Same as (A) for B/plasma, myeloid, proximal tubule, loop of Henle, distal nephron, endothelial/stromal, and glomerular cells, respectively.\", \"page\": 55, \"index\": 4, \"width\": 1058, \"height\": 1075}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-005.webp\", \"caption\": \"Fig. 3. Tissue Specificity Metric. (A) UMAPs of TSM score for immune cells from kidney tissue for B cells (left), myeloid cells (center) and T and NK cells (right). (B-D) Tissue specificity metric of tissue and blood immune cells stratified by cluster for B cells (B), Myeloid cells (C), and T and NK cells (D).\", \"page\": 56, \"index\": 5, \"width\": 979, \"height\": 1137}]"
motivation: 狼疮性肾炎（LN）是一种异质性疾病，其驱动细胞类型尚不明确，需要深入解析以寻找治疗靶点。
method: 对155名LN患者和30名对照的肾脏活检样本及部分患者的血液样本进行了单细胞测序分析。
result: 发现了与疾病活动相关的关键组织细胞状态和免疫细胞群，特别是疤痕相关巨噬细胞（SAMs）在活动性疾病中显著浸润肾小球并驱动纤维化。
conclusion: 靶向巨噬细胞可能是治疗狼疮性肾炎的新策略。
---

## 摘要
单句总结：通过对狼疮性肾炎患者和健康对照者的配对血液和组织样本进行单细胞图谱分析，识别出肾组织内的基质细胞和免疫细胞群体，包括与肾脏疾病活动性相关并可能驱动其发展的瘢痕相关巨噬细胞群体。

狼疮性肾炎（LN）是系统性红斑狼疮（SLE）的一种严重表现，是一种由多种免疫和组织细胞类型驱动的异质性疾病。我们从155名LN患者和30名移植前活检对照者的肾脏活检样本中获得了538K个单细胞和140K个单核转录组数据，同时从与这些患者重叠的样本中获得了325K个单细胞血液转录组数据。我们识别了关键的组织细胞类型、细胞状态以及免疫细胞状态；能够确定组织特异性的细胞状态以及血液中存在的细胞状态。通过差异基因表达分析和协变邻域分析（CNA），我们观察到LN病理特征与特定细胞状态显著相关。这些分析揭示了与不可逆慢性组织损伤相关的广泛细胞状态变化。在控制持续组织损伤的影响后，我们发现关键的肾小球巨噬细胞和瘢痕相关巨噬细胞（SAMs）群体的扩增与炎症性疾病活动性的增加同步。SAMs似乎驱动LN纤维化，并且在活动性疾病中比其他髓系细胞更易浸润肾小球。这些观察结果强烈支持针对髓系细胞的治疗靶向可能为预防LN肾脏炎症和持续肾损伤提供一种尚未被证实的策略。

## Abstract
One Sentence SummaryA single-cell atlas of paired blood and tissue samples from Lupus Nephritis patients and healthy controls identified stromal and immune populations within renal tissue, including the scar-associated macrophage populations, which correlate with and may drive renal disease activity.

Lupus nephritis (LN), a severe manifestation of Systemic Lupus Erythematosus (SLE), is a heterogeneous disease driven by diverse immune and tissue cell types. We obtained 538K single-cell and 140K single-nuclear profiles from kidney biopsies of 155 LN patients and 30 pre-implantation transplant biopsy controls, along with 325K single-cell blood profiles overlapping many of these patients. We identified key tissue cell types and cell states, and immune cell states; we were able to determine cell states that were tissue specific, and those that were present in the blood. We observed that LN pathological features are significantly associated with cell states using differential gene expression and Covarying Neighborhood Analysis (CNA). These analyses revealed broad changes in cell states associated with irreversible chronic tissue damage. After controlling for the effects of ongoing tissue damage, we observed that expansion of key glomerular and Scar Associated Macrophages (SAMs) populations tracked with increasing inflammatory disease activity. SAMs appear to drive LN fibrosis and, in active disease, infiltrate the glomeruli more than other myeloid cells. These observations strongly support that therapeutic targeting of myeloid populations may offer an as-of-yet unproven strategy to prevent renal inflammation and ongoing kidney damage in LN.

---

## 论文详细总结（自动生成）

### 论文分析总结：狼疮性肾炎的血液与组织群体规模图谱

#### 1. 核心问题与整体含义
*   **研究动机**：狼疮性肾炎（LN）是系统性红斑狼疮（SLE）最严重的并发症之一，具有高度异质性，其驱动疾病进展的具体细胞类型和分子机制尚不明确，这阻碍了有效治疗策略的开发。
*   **整体含义**：本研究旨在通过构建大规模的单细胞转录组图谱，系统性地解析LN患者肾脏组织和外周血中的细胞组成与状态变化，以识别与疾病活动、慢性损伤和纤维化相关的关键细胞群体，为发现新的治疗靶点提供依据。

#### 2. 方法论
*   **核心思想**：通过对大量LN患者和健康对照的配对肾脏活检组织与外周血样本进行单细胞及单核RNA测序（scRNA-seq, snRNA-seq），构建高分辨率的细胞图谱，并结合临床病理数据，鉴定与疾病表型相关的特异性细胞状态。
*   **关键技术细节**：
    1.  **单细胞/单核测序**：对155名LN患者和30名对照的肾脏活检样本进行测序，获得约538K个单细胞和140K个单核转录组数据；同时对部分患者的血液样本进行测序，获得约325K个单细胞数据。
    2.  **生物信息学分析流程**：包括标准的数据质控、整合、聚类、细胞类型注释。
    3.  **差异分析与关联研究**：
        *   使用差异基因表达分析寻找不同临床组别间的基因表达变化。
        *   应用**协变邻域分析（Covarying Neighborhood Analysis, CNA）** ，这是一种空间统计方法，用于在单细胞水平上检测特定细胞状态或邻域与临床表型（如疾病活动指数、慢性化指数）之间的关联，并控制多重检验。

#### 3. 实验设计
*   **数据集/场景**：
    *   **主要队列**：155名狼疮性肾炎（LN）患者的肾脏活检组织及部分配对血液样本。
    *   **对照组**：30名肾移植前的健康供体肾脏活检样本作为对照。
    *   **临床表型数据**：包括疾病活动性指数、慢性化指数等病理评分。
*   **Benchmark与对比方法**：本研究属于探索性和描述性研究，旨在构建图谱并发现关联，而非开发预测模型。因此，文中未设置与传统计算方法的横向对比。其“基准”更多是建立在与健康对照组的比较上，以识别疾病特异性的改变。

#### 4. 资源与算力
论文未明确说明数据分析所消耗的具体算力资源（如CPU/GPU型号、数量、计算时长）。可以推断如此大规模的单细胞数据分析（总计超过百万个细胞的测序数据处理、整合和复杂统计）需要在高性能计算集群上完成。

#### 5. 实验数量与充分性
*   **实验数量与分析维度**：
    1.  **基础图谱构建**：对组织和血液中的所有主要细胞类型进行了全面的注释和可视化。
    2.  **差异关联分析**：
        *   病例 vs. 对照的全局关联分析。
        *   针对特定临床表型（疾病活动指数、慢性化指数）的关联分析，并控制了活检部位、慢性化程度等协变量。
        *   分析了不同免疫细胞亚群的组织特异性。
    3.  **关键发现聚焦**：对识别出的重要细胞群（如疤痕相关巨噬细胞SAMs）进行了深入的功能和定位分析（如其在肾小球中的浸润情况）。
*   **充分性与客观性评估**：
    *   **样本量充足**：患者队列规模（n=155）在单细胞研究中属于大型队列，增强了统计效力。
    *   **对照设置合理**：使用了健康的移植前肾脏作为对照，能较好反映生理状态。
    *   **分析方法严谨**：使用了CNA等高级统计方法控制假阳性，并考虑了多种临床协变量。实验设计侧重于观察性关联发现，结论客观地表述为“可能驱动”、“支持靶向…的策略”，并未过度宣称因果关系。

#### 6. 主要结论与发现
1.  成功构建了迄今为止规模最大的LN肾脏组织和血液的单细胞转录组图谱。
2.  发现了广泛的与不可逆慢性组织损伤相关的细胞状态变化。
3.  鉴定出关键的肾小球巨噬细胞和**疤痕相关巨噬细胞（SAMs）群体在活动性疾病中显著扩增。**
4.  SAMs在活动性疾病中更多地浸润肾小球，并且可能驱动肾脏纤维化进程。
5.  研究结果表明，靶向髓系免疫细胞（特别是巨噬细胞）可能是预防LN肾脏炎症和持续损伤的一种有潜力的新治疗策略。

#### 7. 优点
*   **规模性与系统性**：大样本量的配对组织和血液图谱为理解LN提供了前所未有的广度和深度资源。
*   **临床关联性强**：将高维单细胞数据与详细的临床病理指标紧密结合，使生物学发现具有明确的临床意义。
*   **技术方法先进**：应用CNA等方法进行表型-细胞的精细关联定位，超越了传统的批量或平均化分析。
*   **转化医学价值明确**:直接指向了可干预的潜在治疗靶点——巨噬細胞。

####8\.不足與局限\*
\*\*\*\*\*\*\*\*\*\*\*\*\*
\*
\*
\*
\*
\*

(完)

#### 8. 不足与局限
*   **观察性研究的本质**：本研究揭示了丰富的关联性，但无法直接证明因果关系。例如，SAMs的扩增是驱动纤维化的原因，还是纤维化微环境的结果，需要后续的功能性实验验证。
*   **空间信息的缺失**：单细胞测序技术本身丢失了细胞在原组织中的空间位置信息。虽然通过计算推断和已知标记物进行了讨论（如SAMs在肾小球中的浸润），但缺乏直接的、高分辨率的空间转录组证据来精确描绘细胞间的相互作用和微环境。
*   **动态过程的静态快照**：所有分析基于单一时点的活检样本，这提供了一个横断面视图，但无法捕捉LN疾病进展和治疗响应过程中的动态细胞状态变化。纵向样本分析将极大增强研究的说服力。
*   **队列异质性的影响**：尽管大样本量是优势，但LN患者群体在疾病活动度、病理分型、治疗方案和病程上存在高度异质性。虽然研究尝试通过统计方法控制部分协变量，但残余的异质性可能仍会影响某些关联信号的清晰度。
*   **技术偏差的可能性**：单核RNA测序（snRNA-seq）可能对某些脆弱的细胞类型（如高度活化的免疫细胞）捕获效率不足或存在转录本偏好。组织解离过程也可能引入技术性偏差。

#### 9. 总结与展望
本研究通过构建大规模的单细胞转录组图谱，系统性地描绘了狼疮性肾炎肾脏和血液中的免疫景观与实质细胞状态，将特定的髓系细胞群体（尤其是疤痕相关巨噬细胞SAMs）与疾病活动和慢性损伤紧密联系起来。这项工作不仅为理解LN的复杂病理机制提供了宝贵的资源，更重要的是指明了靶向巨噬细胞亚群作为潜在治疗新策略的方向。

未来的研究可以：
1.  **整合空间多组学**：应用空间转录组或成像质谱流式技术，在原位验证并精确解析关键细胞群体（如SAMs）的空间分布、邻居关系及其在组织结构破坏中的作用。
2.  **开展纵向与干预性研究**：收集治疗前后或疾病不同阶段的配对样本，追踪细胞状态的动态演变，并评估针对巨噬细胞的治疗策略在临床试验中的效果与机制。
3.  **深入机制探索**：利用动物模型或体外实验，功能性地验证SAMs等候选细胞群体在驱动炎症和纤维化中的具体分子机制。
4.  **探索临床应用**：基于发现的生物标志物（如特定的巨噬细胞基因特征），开发可用于疾病分型、活动度评估或预后预测的简化检测 panel。

（完）
