---
title: A population-scale atlas of blood and tissue in lupus nephritis
title_zh: 狼疮性肾炎血液与组织的群体规模图谱
authors: "Sugiarto, N. W., Gurajala, S., Curtis, M., Eisenhaure, T. M., Arazi, A., Fava, A., Xiao, Q., Mears, J., Rovin, B., Berthier, C. C., Zhao, Y., Izmirly, P. M., Barnas, J. L., Hoover, P. J., Peters, M., Raychowdhury, R., Horisberger, A., Sakaue, S., Furie, R. A., Belmont, H. M., Hildeman, D. A., Woodle, E. S., Dall'Era, M., Putterman, C., Kamen, D. L., McMahon, M. A., Grossman, J., Kalunian, K. C., Hodgin, J. B., Payan-Schober, F., Apruzzese, W., Perlman, H., Cuda, C. M., Wofsy, D., Guthridge, J. M., Anolik, J. H., James, J. A., Accelerating Medicines Partnerships Rheumatoid Arthritis/Systemic Lu"
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.1101/2025.08.11.669754v3.full.pdf"
tags: ["query:q6"]
score: 9.0
evidence: 狼疮性肾炎单细胞图谱，识别肾活检中的免疫和组织细胞状态
tldr: 本研究构建了狼疮肾炎患者血液和组织的单细胞图谱，通过对155名患者和30名对照的肾脏活检及血液样本进行大规模单细胞测序，鉴定了肾脏组织中的基质和免疫细胞群。研究发现瘢痕相关巨噬细胞群与肾脏疾病活动相关，可能驱动肾纤维化，这为靶向髓系细胞的治疗策略提供了依据。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-001.webp\", \"caption\": \"Fig. 4. Case-control associations within cell types. A-G CNA results for case-control association with no covariate corrections, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with LN, with FDR cutoff of 0.05. Blue and red denote contracted and expanded neighborhoods that pass\", \"page\": 58, \"index\": 1, \"width\": 979, \"height\": 1147}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-002.webp\", \"caption\": \"Fig. 6. Cell states associated with activity index. (A), Across all cell types, CNA results for activity index association while adjusting for first biopsy, site, and chronicity index, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with activity index, with FDR cutoff of 0.1. Dashed vertical lines represent the correlation threshold with FDR < 0.1. Non-significant associations are colored in grey. P-value is the global P-value for cell state associations with activity index phenotype. Right - violin plots of clusters containing cells passing FDR significance for activity index association. (B), Same\", \"page\": 62, \"index\": 2, \"width\": 979, \"height\": 1020}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-003.webp\", \"caption\": \"Fig. 5. Cell states associated with chronicity index. (A), Univariate CNA of each cell type testing for relevant clinical and demographic variables. * indicates a global p-value < 0.05. (B), For each cell\", \"page\": 60, \"index\": 3, \"width\": 979, \"height\": 1099}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-004.webp\", \"caption\": \"Fig. 2. Cell state annotations in tissue. (A) UMAP of T/NK cell states in tissue, colored by fine grain cell state annotations. Annotation boxes are located at the centroid (mean) of each cluster. (B-H), Same as (A) for B/plasma, myeloid, proximal tubule, loop of Henle, distal nephron, endothelial/stromal, and glomerular cells, respectively.\", \"page\": 55, \"index\": 4, \"width\": 1058, \"height\": 1075}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-005.webp\", \"caption\": \"Fig. 3. Tissue Specificity Metric. (A) UMAPs of TSM score for immune cells from kidney tissue for B cells (left), myeloid cells (center) and T and NK cells (right). (B-D) Tissue specificity metric of tissue and blood immune cells stratified by cluster for B cells (B), Myeloid cells (C), and T and NK cells (D).\", \"page\": 56, \"index\": 5, \"width\": 979, \"height\": 1137}]"
motivation: 狼疮肾炎是一种异质性疾病，需要深入了解其驱动细胞类型以开发新疗法。
method: 对155名LN患者和30名对照的肾脏活检样本进行单细胞和单核测序，并结合血液样本分析。
result: 发现与疾病活动相关的关键组织细胞状态，特别是瘢痕相关巨噬细胞在肾小球中的浸润与纤维化驱动作用。
conclusion: 靶向髓系细胞群可能成为预防狼疮肾炎肾脏炎症和损伤的新治疗策略。
---

## 摘要
一句话总结：通过对狼疮性肾炎患者和健康对照者的配对血液和组织样本进行单细胞图谱分析，识别出肾组织内的基质和免疫细胞群，包括与肾脏疾病活动性相关并可能驱动其发展的瘢痕相关巨噬细胞群。

狼疮性肾炎（LN）是系统性红斑狼疮（SLE）的一种严重表现，是一种由多种免疫和组织细胞类型驱动的异质性疾病。我们从155名LN患者和30名移植前对照者的肾活检组织中获得了538K个单细胞和140K个单核转录组数据，并与其中许多患者重叠的325K个血液单细胞数据相结合。我们识别了关键的组织细胞类型、细胞状态以及免疫细胞状态；能够确定哪些是组织特异性的细胞状态，哪些也存在于血液中。通过差异基因表达分析和协变邻域分析（CNA），我们观察到LN病理特征与特定细胞状态显著相关。这些分析揭示了与不可逆的慢性组织损伤相关的广泛细胞状态变化。在控制了持续组织损伤的影响后，我们观察到关键的肾小球和瘢痕相关巨噬细胞（SAMs）群体的扩增与炎症性疾病活动性的增加同步。SAMs似乎驱动LN纤维化，并且在活动性疾病中比其他髓系细胞更多地浸润肾小球。这些观察结果有力地支持了靶向髓系细胞的治疗策略可能为预防LN的肾脏炎症和持续肾损伤提供一种尚未被证实的潜在方法。

## Abstract
One Sentence SummaryA single-cell atlas of paired blood and tissue samples from Lupus Nephritis patients and healthy controls identified stromal and immune populations within renal tissue, including the scar-associated macrophage populations, which correlate with and may drive renal disease activity.

Lupus nephritis (LN), a severe manifestation of Systemic Lupus Erythematosus (SLE), is a heterogeneous disease driven by diverse immune and tissue cell types. We obtained 538K single-cell and 140K single-nuclear profiles from kidney biopsies of 155 LN patients and 30 pre-implantation transplant biopsy controls, along with 325K single-cell blood profiles overlapping many of these patients. We identified key tissue cell types and cell states, and immune cell states; we were able to determine cell states that were tissue specific, and those that were present in the blood. We observed that LN pathological features are significantly associated with cell states using differential gene expression and Covarying Neighborhood Analysis (CNA). These analyses revealed broad changes in cell states associated with irreversible chronic tissue damage. After controlling for the effects of ongoing tissue damage, we observed that expansion of key glomerular and Scar Associated Macrophages (SAMs) populations tracked with increasing inflammatory disease activity. SAMs appear to drive LN fibrosis and, in active disease, infiltrate the glomeruli more than other myeloid cells. These observations strongly support that therapeutic targeting of myeloid populations may offer an as-of-yet unproven strategy to prevent renal inflammation and ongoing kidney damage in LN.

---

## 论文详细总结（自动生成）

# 论文结构化总结：狼疮性肾炎血液与组织的群体规模图谱

## 1. 核心问题与整体含义
**研究动机与背景**：
- **核心问题**：狼疮性肾炎（LN）是系统性红斑狼疮（SLE）最严重的并发症之一，具有高度的临床和病理异质性。现有免疫抑制疗法效果不一，且超过15%的患者会进展至终末期肾病。目前对驱动LN的特定细胞类型和状态，尤其是在肾脏组织微环境中的动态变化，缺乏系统、深入的理解。
- **研究目标**：构建一个大规模、高分辨率的单细胞图谱，系统描绘LN患者肾脏组织和外周血中的细胞组成与状态，并阐明这些细胞状态如何与关键的临床病理指标（如活动性指数、慢性化指数）相关联，以识别潜在的致病细胞群和治疗靶点。

## 2. 方法论
**核心思想与技术细节**：
- **数据生成与整合**：
    - **样本来源**：收集了155名LN患者和30名健康对照的肾活检组织，以及其中118名LN患者和19名对照的配对外周血单个核细胞（PBMC）。
    - **测序技术**：对肾组织同时进行**单细胞RNA测序（scRNA-seq）** 和**单核RNA测序（snRNA-seq）**，以互补地捕获对组织解离敏感的细胞类型（如免疫细胞）和脆弱的实质细胞。对PBMC进行scRNA-seq。
    - **数据规模**：最终数据集包含肾组织中的538,194个scRNA-seq图谱和142,881个snRNA-seq图谱，以及PBMC中的327,326个scRNA-seq图谱。
- **数据分析流程**：
    1.  **质量控制与整合**：去除低质量细胞后，使用加权主成分分析（PCA）结合Harmony算法整合scRNA-seq和snRNA-seq数据，以平衡不同技术带来的偏差。
    2.  **细胞注释与聚类**：首先鉴定出8个主要细胞大类（3类免疫细胞：T/NK、B/浆细胞、髓系；5类肾实质细胞：肾小球、近端小管、亨利袢、远端肾单位、内皮/基质），然后对每大类进行精细亚聚类，共定义了55个免疫亚群和36个实质亚群。
    3.  **组织特异性度量（TSM）**：通过整合肾脏和血液的免疫细胞数据，计算每个细胞的TSM分数（基于其k近邻中来自组织的比例），以区分组织驻留型、血液型及共享型免疫状态。
    4.  **统计关联分析 - 协变邻域分析 (CNA)**：
        - **核心思想**：CNA不依赖于离散的聚类结果，而是将转录相似的单个细胞划分为微小的“邻域”，然后检验每个样本中这些邻域的丰度是否与样本层面的表型变量显著相关。这种方法克服了多重假设检验的统计效力限制。
        - **应用场景**：用于系统评估病例vs对照状态、慢性化指数、活动性指数等临床病理变量与所有精细细胞状态之间的关联。
    5.  **差异基因表达与通路富集分析 (GSEA)**：基于伪批量数据进行差异表达分析。
    6.  **轨迹推断 (Pseudotime Analysis)**：使用Destiny进行降维和Slingshot推断B细胞和髓系细胞的潜在分化轨迹。
    7.  **空间转录组学验证与定位**：利用一个外部儿童期发病SLE的空间转录组数据集（7例 vs 4对照），训练逻辑回归分类器将本研究鉴定的瘢痕相关巨噬群映射到空间位置。

## 3. 实验设计
- **主要数据集/场景**: 
    - AMP SLE/LN前瞻性队列的肾活检组织和配对PBMC样本。这是一个大型、多中心的临床队列。
    - ISN/RPS III, IV, V类或混合型LN患者；健康对照为移植前供体肾活检样本。
- **Benchmark/对比方法**: 
    - 本研究是描述性和发现性的资源构建工作，并非旨在提出一个新算法并与现有方法比较性能。其主要“对比”在于：
        1.  病例 vs. 健康对照的比较分析。
        2.  不同临床病理指标（如活动性 vs. 慢性化指数；ISN分型 vs. NIH指数）在解释分子表型上的相对重要性比较。
        3.  将自身单核数据结果与外部的空间转录组数据进行交叉验证，评估技术偏差并确认关键发现的空间定位。

## 4. 资源与算力
- **算力信息**: 
    -论文正文及方法部分未明确提及具体使用的GPU型号、数量或训练时长等计算资源细节。考虑到处理近百万级单细胞的复杂整合与分析流程（Harmony, CNA, UMAP等），可以推断其计算需求是巨大的。

## 5.实验数量与充分性
-实验数量庞大且设计系统：
1.**基础表征实验**:对所有样本进行了全面的单/核测序及基础注释(图1)。
2.**病例对照关联分析**:在所有主要及精细亚群水平进行了CNA(图4)。
3.**临床变量关联分析**:系统地测试了年龄性别活动性慢性化ISN分型首次活检状态等多个变量对所有主要及精细亚群的独立影响(图5A)。
4.**关键变量深入剖析**:针对慢性化和活动性这两个最重要的指标分别进行了深入的CNA差异表达GSEA轨迹分析和空间验证(图56及相关附图)。
5.**控制混淆因素**:在关键分析中均校正了首次活检状态招募地点等潜在混淆因素确保了结果的稳健性(图S23D)。
6.**技术验证与控制实验**:比较了sc/sn两种技术的捕获偏好性与外部空间数据的比例一致性(图S12-S13)进行了下采样敏感性测试(图S21)并使用CITE-Seq验证了PBMC注释(图S37)。

-**充分性与客观公平性评价**
该研究实验设计全面覆盖了从基础描述到机制探索再到外部验证的全链条分析方法选择恰当(CNA尤其适合此类探索)且考虑了多种技术偏差和控制因素结果呈现客观例如明确指出了B细胞的低频可能限制了其发现能力也承认了单核技术在捕获某些实质细胞的局限性总体而言实验充分论证严谨。

##6论文的主要结论与发现
-**关键发现**
1.**构建了一个全面的LN单/核及血液图谱资源**
定义了91个精细的肾脏免疫和组织亚群为领域提供了宝贵的参考数据集。

2.**揭示了疾病相关的关键免疫和组织状态**
包括自身免疫相关BABCs近端小管损伤态PT0以及一系列组织特异性巨噬群如GPNMB高巨噬M5M11SPP1高FABP5高巨噬M7。

3.**明确了不同临床变量的分子相关性**
-**慢性化指数影响最广泛**:主要反映不可逆的组织损伤特别是近端小管损伤态PT0的扩增可作为其分子代理物同时伴随特定髓系T/NK细胞的扩增这些变化在很大程度上独立于治疗反应提示其代表累积的组织损害而非可逆炎症过程
-**活动性指数关联更特异性地指向髓系和肾小球**
即使校正慢性化后活动性的升高仍特异地伴随着一组瘢痕相关巨噬SAMs包括M5M7M9M11以及活化的小球壁上皮GLOM1的扩增SAMs表达CD9GPNMBFABP5TREM2SPP1等标志物并通过空间分析和受体配体互作预测显示其在活动性疾病中优先浸润肾小球并与GLOM1通过SPP1/TNC介导的上皮间质转化EMT通路相互作用可能驱动纤维化

4.**阐明了血液组织的异同**
血液能有效区分病例对照并显示干扰素信号上调但几乎无法反映肾脏的活动性或慢性化程度强调了直接研究病变组织的必要性

5.**挑战了传统分类体系的价值**
研究发现相较于ISN分型NIH的活动性和慢性化指数能更好地解释肾脏组织的分子表型变化例如V类膜性肾病相关的分子改变主要由其较低的活动性而非特定的病理分型本身所解释

-**核心结论**
SAMs是与LN疾病活动密切相关的关键致病候选群体靶向髓系特别是SAMs可能为预防肾脏炎症和纤维化提供新的治疗策略而传统的ISN分型在指导精准治疗方面的价值可能低于直接评估组织炎症活性

##7优点
-**规模宏大资源宝贵**:迄今为止最大的LN肾脏单/核测序队列之一结合配对血液数据构成了极具价值的公共资源
-**技术互补设计严谨**:同时采用sc/sn两种方法减少了单一技术的捕获偏倚提高了注释可靠性
-**分析方法先进适用性强**:采用CNA进行无偏见的表型关联分析避免了离散聚类的主观性和统计效力问题特别适合探索异质性疾病
-**多层次交叉验证**:结合内部的下采样敏感性测试外部的空间转录组学验证以及受体配体互作预测使关键发现更具说服力
-**临床转化意义明确**:直接将分子特征链接到关键的预后指标活动性和慢性化为开发新的生物标志物和治疗靶点提供了清晰的方向

##8不足与局限
-**横断面研究的固有局限**:无法确定观察到的关联是因果关系还是继发性改变缺乏纵向随访样本来追踪动态变化
-**B细胞的低频限制了发现能力**:尽管通过与空间数据对比排除了主要的技术原因但组织中B细胞的绝对数量少可能掩盖了一些重要的疾病相关罕见B细胞亚群这与B细胞作为重要治疗靶点的现状形成反差提示其在肾脏局部的作用方式可能需要重新审视或通过其他途径研究例如淋巴结)
-**解离过程可能导致比例失真**:尽管使用了sn补充但仍观察到某些实质特别是肾小球内皮基质细胞的相对比例低于空间数据这可能会影响对这些群体绝对丰度的解读)
-**缺乏蛋白层面的验证注释仅基于转录组虽然使用了已知标记基因但结合表面蛋白标记如CITE-Seq可进一步提高免疫亚群注释的准确性)
-**队列异质性带来的复杂性患者处于不同的疾病阶段接受不同的治疗方案虽然这是真实世界研究的优势但也增加了分离药物效应和其他混杂因素的难度)
-SAMs的非特异性:作者指出SAMs也可能存在于其他器官纤维化和肾病中未来需要与其他肾病进行比较研究以确定其在LN中的特异性)

完

## 9. 总结与展望
-**总结**：本研究通过构建大规模、高分辨率的单细胞图谱，系统揭示了LN肾脏微环境中细胞组成的深刻变化，并成功地将特定的细胞状态（如PT0、SAMs）与关键的临床病理指标（活动性、慢性化指数）联系起来。它挑战了传统病理分型在反映分子机制上的局限性，并突出了组织驻留髓系细胞，特别是瘢痕相关巨噬细胞（SAMs），在驱动疾病活动性和纤维化中的核心作用。
-**未来方向**：
    1.  **纵向与干预研究**：需要在纵向队列中验证这些细胞状态的动态变化，并在治疗干预（如使用抗CD20或抗IFNAR抗体）前后进行采样，以明确其因果作用和作为治疗反应标志物的潜力。
    2.  **机制深入探索**：对关键群体（如SAMs、PT0）进行功能实验，验证其通过SPP1-TNC等通路促进纤维化的机制，并利用基因工程小鼠模型进行体内验证。
    3.  **跨疾病比较**：将本研究发现的“瘢痕相关”特征与其他慢性肾病（如糖尿病肾病、IgA肾病）的单细胞图谱进行比较，以确定LN特异性的靶点。
    4.  **技术整合与提升**：结合空间蛋白质组学（如CODEX）、谱系追踪等技术，在空间和时间维度上更精确地解析细胞互作与命运转变。
    5.  **临床转化**：开发基于血液或尿液的无创检测方法，来监测肾脏内SAMs或PT0相关信号，并将其用于临床试验的患者分层和疗效评估。

本研究为理解LN的异质性提供了前所未有的精细视角，为未来开发针对特定致病细胞状态的精准疗法奠定了坚实的分子基础。

（完）
