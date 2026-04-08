---
title: A population-scale atlas of blood and tissue in lupus nephritis
title_zh: 狼疮性肾炎血液与组织的群体规模图谱
authors: "Sugiarto, N. W., Gurajala, S., Curtis, M., Eisenhaure, T. M., Arazi, A., Fava, A., Xiao, Q., Mears, J., Rovin, B., Berthier, C. C., Zhao, Y., Izmirly, P. M., Barnas, J. L., Hoover, P. J., Peters, M., Raychowdhury, R., Horisberger, A., Sakaue, S., Furie, R. A., Belmont, H. M., Hildeman, D. A., Woodle, E. S., Dall'Era, M., Putterman, C., Kamen, D. L., McMahon, M. A., Grossman, J., Kalunian, K. C., Hodgin, J. B., Payan-Schober, F., Apruzzese, W., Perlman, H., Cuda, C. M., Wofsy, D., Guthridge, J. M., Anolik, J. H., James, J. A., Accelerating Medicines Partnerships Rheumatoid Arthritis/Systemic Lu"
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.1101/2025.08.11.669754v3.full.pdf"
tags: ["query:q6"]
score: 8.0
evidence: 狼疮性肾炎肾活检单细胞图谱，识别免疫和组织细胞状态
tldr: 本研究通过构建狼疮性肾炎（LN）患者血液和肾脏组织的单细胞图谱，揭示了疾病中免疫和组织细胞的异质性。利用155名LN患者和30名对照的样本进行单细胞测序，结合共变邻域分析，识别出与不可逆慢性组织损伤相关的细胞状态变化。研究发现瘢痕相关巨噬细胞（SAMs）在活动性疾病中显著浸润肾小球，并与纤维化进程相关，提示靶向髓系细胞群可能成为预防肾脏炎症和损伤的新治疗策略。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-001.webp\", \"caption\": \"Fig. 4. Case-control associations within cell types. A-G CNA results for case-control association with no covariate corrections, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with LN, with FDR cutoff of 0.05. Blue and red denote contracted and expanded neighborhoods that pass\", \"page\": 58, \"index\": 1, \"width\": 979, \"height\": 1147}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-002.webp\", \"caption\": \"Fig. 6. Cell states associated with activity index. (A), Across all cell types, CNA results for activity index association while adjusting for first biopsy, site, and chronicity index, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with activity index, with FDR cutoff of 0.1. Dashed vertical lines represent the correlation threshold with FDR < 0.1. Non-significant associations are colored in grey. P-value is the global P-value for cell state associations with activity index phenotype. Right - violin plots of clusters containing cells passing FDR significance for activity index association. (B), Same\", \"page\": 62, \"index\": 2, \"width\": 979, \"height\": 1020}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-003.webp\", \"caption\": \"Fig. 5. Cell states associated with chronicity index. (A), Univariate CNA of each cell type testing for relevant clinical and demographic variables. * indicates a global p-value < 0.05. (B), For each cell\", \"page\": 60, \"index\": 3, \"width\": 979, \"height\": 1099}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-004.webp\", \"caption\": \"Fig. 2. Cell state annotations in tissue. (A) UMAP of T/NK cell states in tissue, colored by fine grain cell state annotations. Annotation boxes are located at the centroid (mean) of each cluster. (B-H), Same as (A) for B/plasma, myeloid, proximal tubule, loop of Henle, distal nephron, endothelial/stromal, and glomerular cells, respectively.\", \"page\": 55, \"index\": 4, \"width\": 1058, \"height\": 1075}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-005.webp\", \"caption\": \"Fig. 3. Tissue Specificity Metric. (A) UMAPs of TSM score for immune cells from kidney tissue for B cells (left), myeloid cells (center) and T and NK cells (right). (B-D) Tissue specificity metric of tissue and blood immune cells stratified by cluster for B cells (B), Myeloid cells (C), and T and NK cells (D).\", \"page\": 56, \"index\": 5, \"width\": 979, \"height\": 1137}]"
motivation: 研究动机是为了揭示狼疮性肾炎（LN）中驱动肾脏疾病活动的异质性免疫和组织细胞类型，以改善对这种严重疾病的理解和治疗。
method: 研究方法包括对155名LN患者和30名对照的肾脏活检样本进行单细胞和单核测序，并结合血液样本分析，使用差异基因表达和共变邻域分析（CNA）来识别细胞状态。
result: 研究发现关键的组织细胞类型和状态，特别是瘢痕相关巨噬细胞（SAMs）与疾病活动性相关，并可能驱动肾纤维化和炎症。
conclusion: 研究结论表明，靶向髓系细胞群可能为预防狼疮性肾炎的肾脏炎症和持续损伤提供新的治疗策略。
---

## 摘要
单句总结：通过对狼疮性肾炎患者和健康对照者的配对血液和组织样本进行单细胞图谱分析，识别出肾组织内的基质和免疫细胞群体，包括与肾脏疾病活动性相关并可能驱动其发展的瘢痕相关巨噬细胞群体。

狼疮性肾炎（LN）是系统性红斑狼疮（SLE）的一种严重表现，是一种由多种免疫和组织细胞类型驱动的异质性疾病。我们从155名LN患者和30名移植前活检对照者的肾脏活检样本中获得了538K个单细胞和140K个单核转录组数据，同时从与这些患者重叠的样本中获得了325K个单细胞血液转录组数据。我们识别了关键的组织细胞类型、细胞状态以及免疫细胞状态；能够确定组织特异性的细胞状态以及存在于血液中的细胞状态。通过差异基因表达分析和共变邻域分析（CNA），我们观察到LN病理特征与特定细胞状态显著相关。这些分析揭示了与不可逆慢性组织损伤相关的广泛细胞状态变化。在控制持续组织损伤的影响后，我们发现关键的肾小球巨噬细胞和瘢痕相关巨噬细胞（SAMs）群体的扩增与炎症性疾病活动性的增加同步。SAMs似乎驱动LN纤维化，并且在活动性疾病中比其他髓系细胞更易浸润肾小球。这些观察结果强有力地支持了靶向髓系细胞的治疗策略可能为预防LN肾脏炎症和持续肾损伤提供一种尚未被证实的潜在途径。

## 速览
**TLDR**：本研究构建了一个大规模的狼疮肾炎患者配对血液和组织样本的单细胞图谱。通过对155名患者和30名对照的肾脏活检及部分患者血液进行单细胞/单核测序，研究鉴定了肾脏组织内的基质和免疫细胞群体，特别是疤痕相关巨噬细胞。分析发现这些细胞的特定状态与病理特征显著相关，其中疤痕相关巨噬细胞的扩增追踪着炎症活动度的增加，并可能驱动肾纤维化和肾小球浸润。这为靶向髓系细胞的治疗策略提供了新依据。 \
**Motivation**：狼疮肾炎是一种异质性疾病，其驱动机制复杂，本研究旨在通过构建大规模单细胞图谱来解析其肾脏和血液中的关键细胞类型与状态。 \
**Method**：研究对155名狼疮肾炎患者和30名对照的肾脏活检样本及部分患者的血液样本进行了单细胞和单核测序，并运用差异基因表达和共变邻域分析等方法。 \
**Result**：研究发现与不可逆慢性组织损伤相关的广泛细胞状态变化，并识别出关键的肾小球细胞和疤痕相关巨噬细胞亚群，其扩增与炎症活动度增加相关。 \
**Conclusion**：研究结论表明，靶向髓系细胞（如疤痕相关巨噬细胞）可能是一种预防狼疮肾炎肾脏炎症和损伤的新治疗策略。

---

## Abstract
One Sentence SummaryA single-cell atlas of paired blood and tissue samples from Lupus Nephritis patients and healthy controls identified stromal and immune populations within renal tissue, including the scar-associated macrophage populations, which correlate with and may drive renal disease activity.

Lupus nephritis (LN), a severe manifestation of Systemic Lupus Erythematosus (SLE), is a heterogeneous disease driven by diverse immune and tissue cell types. We obtained 538K single-cell and 140K single-nuclear profiles from kidney biopsies of 155 LN patients and 30 pre-implantation transplant biopsy controls, along with 325K single-cell blood profiles overlapping many of these patients. We identified key tissue cell types and cell states, and immune cell states; we were able to determine cell states that were tissue specific, and those that were present in the blood. We observed that LN pathological features are significantly associated with cell states using differential gene expression and Covarying Neighborhood Analysis (CNA). These analyses revealed broad changes in cell states associated with irreversible chronic tissue damage. After controlling for the effects of ongoing tissue damage, we observed that expansion of key glomerular and Scar Associated Macrophages (SAMs) populations tracked with increasing inflammatory disease activity. SAMs appear to drive LN fibrosis and, in active disease, infiltrate the glomeruli more than other myeloid cells. These observations strongly support that therapeutic targeting of myeloid populations may offer an as-of-yet unproven strategy to prevent renal inflammation and ongoing kidney damage in LN.

---

## 论文详细总结（自动生成）

# 论文结构化总结：狼疮性肾炎血液与组织的群体规模图谱

## 1. 核心问题与整体含义
**研究动机与背景**：
- **核心问题**：狼疮性肾炎（LN）是系统性红斑狼疮（SLE）最严重的并发症之一，具有高度的临床和病理异质性。尽管已有多种免疫抑制剂，但超过50%的患者无法达到完全缓解，约15%会进展至终末期肾病。目前对驱动LN肾脏炎症和纤维化的具体细胞类型及其动态变化缺乏系统性、高分辨率的理解。
- **研究目标**：本研究旨在构建一个大规模、高分辨率的单细胞图谱，系统描绘LN患者肾脏组织和外周血中的免疫细胞及实质细胞的精细状态，并阐明这些细胞状态如何与关键的临床病理指标（如活动性指数、慢性化指数）相关联，从而识别潜在的致病细胞群和治疗靶点。

## 2. 方法论
**核心思想与技术细节**：
- **数据生成与整合**：
    - **技术平台**：对肾脏活检组织同时进行单细胞RNA测序（scRNA-seq）和单核RNA测序（snRNA-seq），以克服组织解离对脆弱细胞类型（如实质细胞）的偏好性损失。
    - **样本匹配**：收集了155名LN患者和30名健康对照的肾脏样本，并对其中118名患者和19名对照匹配了外周血单个核细胞（PBMC）样本。
    - **数据规模**：最终数据集包含来自肾脏组织的538,194个scRNA-seq图谱和142,881个snRNA-seq图谱，以及来自血液的327,326个scRNA-seq图谱。
- **数据分析流程**：
    1.  **质量控制与整合**：使用加权主成分分析（wPCA）结合Harmony算法整合scRNA-seq和snRNA-seq数据，校正批次和技术差异。
    2.  **细胞注释与聚类**：首先鉴定8个主要细胞大类（3类免疫细胞：T/NK、B/浆细胞、髓系；5类肾实质细胞：肾小球、近端小管、髓袢、远端肾单位、内皮/基质），然后对每类进行精细亚群聚类，共定义了91个精细细胞状态。
    3.  **组织特异性分析**：通过整合肾脏和血液的免疫细胞数据，计算“组织特异性指标”（TSM），量化每个免疫细胞状态在组织和血液中的分布倾向。
    4.  **统计关联分析 - CNA (Covarying Neighborhood Analysis)**：
        - **核心思想**：克服传统基于离散聚类的多重假设检验效力不足的问题。CNA将转录相似的单个细胞的邻域作为分析单元，检验这些邻域的丰度是否与样本水平的表型变量显著相关。
        - **流程简述**：
            a. 在低维嵌入空间（如Harmony校正后的PCs）中定义大量细粒度的“邻域”。
            b. 计算每个样本中每个邻域的丰度。
            c. 使用回归模型检验邻域丰度与临床变量（如病例/对照状态、活动性指数、慢性化指数）的关联性，并计算全局显著性p值。
            d. 将显著相关的邻域映射回已注释的细胞簇上，进行生物学解释。
    5.  **其他分析**：
        - **差异基因表达分析 (DGE)**：基于伪批量计数进行负二项回归模型分析。
        - **轨迹推断 (Pseudotime)**：使用Destiny进行扩散图降维，Slingshot推断分化轨迹。
        - **空间转录组学验证**：利用外部空间转录组数据集训练逻辑回归分类器，验证关键巨噬群落在肾小球中的定位。

## 3. 实验设计
- **数据集/场景**：
    - **主要队列 (AMP SLE Cohort)**：155名经活检确诊的LN患者（ISN III, IV, V类或混合型）和30名健康活体肾移植供者作为对照。所有患者均有详细的临床病理资料（ISN分型、NIH活动性/慢性化指数等）。
    - **外部验证数据集 (Danaher et al.)**:  一个包含7例儿童期发病SLE和4例对照的980基因CosMX空间转录组数据集，用于验证关键发现的空间定位。
- **Benchmark与对比方法**：
    - 本研究是描述性和探索性的资源构建工作，并非旨在提出并击败某个预测模型。其主要“对比”在于：
        1.  不同技术间的比较：比较了scRNA-seq和snRNA-seq在捕获不同细胞类型比例上的差异；并与空间转录组数据比较了各技术捕获的各类细胞的相对比例。
        2.  不同临床变量解释力的比较：系统比较了ISN分型、活动性指数、慢性化指数等多个临床变量对单细胞表型的解释力强弱。

## 4. 资源与算力
- 论文未明确说明具体的计算硬件配置（如GPU型号、数量）、软件运行时间或总计算成本。文中提及的分析主要依赖于标准的生物信息学流程和高性能计算集群。

## 5.实验数量与充分性
- **实验广度充分且系统性强**
    -  覆盖了从病例/对照到疾病内部分层分析的多个层面：（1）病例 vs. （2）疾病内部分析：（a）慢性化指数，（b）活动性指数，（c）ISN分型，（d）治疗反应等）。
    -  在每个层面均进行了多角度的互补分析：（1) CNA识别关联的细胞状态；（2) DGE揭示相关的基因通路；（3) GSEA富集分析；（4) TSM评估组织驻留特性；（5) Pseudotime推断分化关系；（6)受体-配体互作网络分析等）。
    -  进行了广泛的敏感性分析和混杂因素校正：（1)调整年龄、性别；（2)调整首次活检状态和研究中心效应；（3)通过子抽样平衡病例/对照样本量和细胞数来验证结果的稳健性；（4)针对关键发现进行了独立的空间数据验证。

##6 .主要结论与发现
1.  构建了一个全面的LN单细胞参考图谱:公开提供了包含91个精细定义的肾脏组织和血液免疫细胞的参考图谱资源.
2 .揭示了疾病特异性的关键致病相关群体:
    *  瘢痕相关巨噬群(SAMs):表达GPNMB SPP1 CD9 FABP5 TREM2等标志物(M5 M7 M9 M11).它们随活动性指数的升高而显著扩增能更有效地浸润肾小球并通过分泌SPP1等分子与活化的壁层上皮相互作用可能通过上皮间质转化途径驱动纤维化.
    *  近端小管损伤态(PT0):表达VCAM1 TPM1 DCDC2代表一种适应不良修复或去分化状态其丰度是慢性化指数的强有力分子代理并与广泛的免疫和其他实质细胞的改变相关联.
3 .明确了不同临床指标的解释优先级:在解释单细胞的异质性方面慢性化指数的效应最强最广泛其次是活动性指数而传统的ISN分型的效应在很大程度上可由其伴随的活动性水平来解释.
4 .阐明了组织驻留特性:大多数随疾病严重程度增加的免疫群体(如SAMs特定CD4+记忆T )具有高度的组织特异性而非循环来源.
5 .揭示了血液信号的局限性:尽管血液中可检测到干扰素信号增强等变化但其免疫表型变化仅微弱地反映肾脏慢性化且几乎不反映活动性与组织内的强烈信号形成对比.

##7 .优点
*  规模空前且设计严谨:迄今为止最大的配对血液和组织样本的单cell LN研究队列采用双模态测序(sc/sn RNA seq )有效互补减少了技术偏差.
*  分析方法先进:CNA的应用避免了离散聚类带来的信息损失提高了检测细微但一致的连续变化的统计效力.
*  多层次验证:内部通过双模态一致性检验外部通过独立的空间转录组数据进行定位验证增强了结论的可信度.
*  临床转化意义明确:直接关联经典的病理评分指标使基础发现易于被临床医生理解并直接指向SAMs这一潜在的新型治疗靶点.

##8 .不足与局限
* B细胞的代表性有限:B cell在组织中频率极低(占总细胞的~2%)尽管通过与空间数据比对排除了主要的技术原因但这限制了对其在局部致病作用的深入探究可能反映了其在淋巴结等其他部位更活跃的现实.
*采样偏差与技术限制:
      *单cell方法可能导致某些脆弱或粘连紧密的群体丢失例如肾小球细胞的相对比例低于空间数据.
      *缺乏表面蛋白标记仅依赖转录组数据进行免疫分型可能存在一定的不确定性.
      *研究为横断面设计无法确定识别的关联是因果关系还是结果;缺乏纵向随访样本以追踪动态变化.
*队列异质性:患者处于不同的疾病阶段接受不同的治疗方案虽然这是真实世界研究的优势但也增加了混杂因素分析的复杂性即使已尽力校正残余混杂仍可能存在.

(完)

## 9. 潜在影响与未来方向
*   **对LN研究领域的影响**：
    *   **提供了核心资源**：本研究构建的公开、交互式图谱将成为未来LN机制研究和生物标志物发现的基石，使研究者能够快速查询特定细胞状态在疾病中的变化。
    *   **重新定义了疾病评估框架**：研究结果表明，基于组织分子表型（如PT0和SAMs的丰度）的评估可能比传统的组织学分类（ISN分型）更能反映疾病的慢性化进程和潜在生物学机制，为开发更精准的病理-分子分型系统提供了数据支持。
    *   **指明了明确的治疗靶点**：瘢痕相关巨噬群（SAMs），特别是其核心信号通路（如SPP1-CD44、TREM2），被确定为连接炎症与纤维化的关键节点，是极具潜力的新型治疗干预靶点。
*   **对更广泛领域的方法学贡献**：
    *   **CNA方法的示范应用**：本研究展示了CNA在解决复杂疾病异质性、关联连续临床表型与单细胞数据方面的强大能力，为其他领域类似研究提供了分析范本。
    *   **多模态整合的范例**：成功整合scRNA-seq、snRNA-seq和空间转录组数据，为全面解析组织微环境树立了技术标杆。
*   **提出的未来研究方向**：
    *   **机制验证与靶点开发**：需要在实验模型（如小鼠模型或类器官）中功能性地验证SAMs和PT0细胞的致病角色，并探索靶向这些细胞或其通路的治疗策略。
    *   **纵向研究与治疗反应预测**：收集治疗前后或疾病复发时的配对样本进行纵向测序，以确定哪些细胞状态可预测治疗反应或复发风险。
    *   **空间多组学深化**：利用更高分辨率的多重成像技术（如CODEX、MIBI）在原位验证关键细胞群体的空间互作关系。
    *   **扩大B细胞研究**：通过富集策略或直接对淋巴组织取样，深入探究B细胞在LN发病中的具体作用。

## 10. 总结
本研究通过构建狼疮性肾炎迄今最大规模的血液与组织单细胞图谱，系统揭示了驱动肾脏损伤与纤维化的核心细胞元件。其核心贡献在于：
1.  **识别出两个关键的致病相关细胞状态**：一是位于肾脏间质、与活动性损伤和纤维化密切相关的“瘢痕相关巨噬群”（SAMs）；二是代表近端小管适应不良修复、作为慢性化进程核心指标的“损伤态近端小管细胞”（PT0）。
2.  **确立了临床-分子关联的新层次**：证明慢性化指数在解释单细胞异质性上具有最强的效力，其分子基础超越了传统的活动性炎症指标，为预后判断提供了更精细的视角。
3.  **凸显了组织局部微环境的核心地位**：大多数致病免疫群体具有高度的组织驻留特性，而外周血免疫谱仅能微弱反映肾脏内部的慢性化进程，强调了针对局部靶点进行治疗的重要性。
4.  **提供了先进的方法学资源**：不仅公开了宝贵的图谱数据，还通过应用CNA等创新分析方法，为从高维单细胞数据中提取具有临床意义的生物学发现提供了强大工具。

总之，这项研究将LN的理解从传统的组织病理学层面推进到了高分辨率的分子细胞层面，为开发基于特定致病细胞状态的精准诊断工具和靶向疗法奠定了坚实的基础。

（完）
