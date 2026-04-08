---
title: A population-scale atlas of blood and tissue in lupus nephritis
title_zh: 狼疮性肾炎血液与组织的群体规模图谱
authors: "Sugiarto, N. W., Gurajala, S., Curtis, M., Eisenhaure, T. M., Arazi, A., Fava, A., Xiao, Q., Mears, J., Rovin, B., Berthier, C. C., Zhao, Y., Izmirly, P. M., Barnas, J. L., Hoover, P. J., Peters, M., Raychowdhury, R., Horisberger, A., Sakaue, S., Furie, R. A., Belmont, H. M., Hildeman, D. A., Woodle, E. S., Dall'Era, M., Putterman, C., Kamen, D. L., McMahon, M. A., Grossman, J., Kalunian, K. C., Hodgin, J. B., Payan-Schober, F., Apruzzese, W., Perlman, H., Cuda, C. M., Wofsy, D., Guthridge, J. M., Anolik, J. H., James, J. A., Accelerating Medicines Partnerships Rheumatoid Arthritis/Systemic Lu"
date: 2026-04-02
pdf: "https://www.biorxiv.org/content/10.1101/2025.08.11.669754v3.full.pdf"
tags: ["query:q6"]
score: 9.0
evidence: 狼疮性肾炎肾活检中的免疫和组织细胞状态
tldr: 本研究构建了狼疮肾炎患者的大规模单细胞图谱，涵盖肾脏组织和血液样本。通过分析发现肾脏内存在基质和免疫细胞群，其中瘢痕相关巨噬细胞（SAMs）与疾病活动性密切相关，可能驱动肾纤维化和炎症。这提示靶向髓系细胞群或可成为治疗狼疮肾炎的新策略。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-001.webp\", \"caption\": \"Fig. 4. Case-control associations within cell types. A-G CNA results for case-control association with no covariate corrections, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with LN, with FDR cutoff of 0.05. Blue and red denote contracted and expanded neighborhoods that pass\", \"page\": 58, \"index\": 1, \"width\": 979, \"height\": 1147}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-002.webp\", \"caption\": \"Fig. 6. Cell states associated with activity index. (A), Across all cell types, CNA results for activity index association while adjusting for first biopsy, site, and chronicity index, in scRNA-seq data. Left - UMAP displaying significant per-cell associations with activity index, with FDR cutoff of 0.1. Dashed vertical lines represent the correlation threshold with FDR < 0.1. Non-significant associations are colored in grey. P-value is the global P-value for cell state associations with activity index phenotype. Right - violin plots of clusters containing cells passing FDR significance for activity index association. (B), Same\", \"page\": 62, \"index\": 2, \"width\": 979, \"height\": 1020}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-003.webp\", \"caption\": \"Fig. 5. Cell states associated with chronicity index. (A), Univariate CNA of each cell type testing for relevant clinical and demographic variables. * indicates a global p-value < 0.05. (B), For each cell\", \"page\": 60, \"index\": 3, \"width\": 979, \"height\": 1099}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-004.webp\", \"caption\": \"Fig. 2. Cell state annotations in tissue. (A) UMAP of T/NK cell states in tissue, colored by fine grain cell state annotations. Annotation boxes are located at the centroid (mean) of each cluster. (B-H), Same as (A) for B/plasma, myeloid, proximal tubule, loop of Henle, distal nephron, endothelial/stromal, and glomerular cells, respectively.\", \"page\": 55, \"index\": 4, \"width\": 1058, \"height\": 1075}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-08-11-669754-v3/fig-005.webp\", \"caption\": \"Fig. 3. Tissue Specificity Metric. (A) UMAPs of TSM score for immune cells from kidney tissue for B cells (left), myeloid cells (center) and T and NK cells (right). (B-D) Tissue specificity metric of tissue and blood immune cells stratified by cluster for B cells (B), Myeloid cells (C), and T and NK cells (D).\", \"page\": 56, \"index\": 5, \"width\": 979, \"height\": 1137}]"
motivation: 狼疮肾炎（LN）是一种异质性疾病，其驱动细胞类型多样，本研究旨在通过构建大规模单细胞图谱来解析其肾脏组织和血液中的关键细胞群与疾病活动的关系。
method: 对155名LN患者和30名对照的肾脏活检样本及部分患者的血液样本进行单细胞和单核测序，共获得约538K个单细胞和140K个单核图谱，并采用差异基因表达和共变邻域分析（CNA）。
result: 研究发现组织特异性免疫细胞状态，特别是瘢痕相关巨噬细胞（SAMs）的扩增与疾病活动性增加相关，且SAMs在活跃疾病中更易浸润肾小球并驱动纤维化。
conclusion: 靶向髓系细胞群可能成为预防狼疮肾炎肾脏炎症和损伤的新治疗策略。
---

## 摘要
单句总结：通过对狼疮性肾炎患者和健康对照者的配对血液和组织样本进行单细胞图谱分析，识别出肾组织内的基质细胞和免疫细胞群体，包括与肾脏疾病活动性相关并可能驱动其发展的瘢痕相关巨噬细胞群体。

狼疮性肾炎（LN）是系统性红斑狼疮（SLE）的一种严重表现，是一种由多种免疫细胞和组织细胞类型驱动的异质性疾病。我们从155名LN患者和30名移植前活检对照者的肾脏活检样本中获得了538K个单细胞和140K个单核转录组数据，同时从与这些患者重叠的样本中获得了325K个单细胞血液转录组数据。我们识别了关键的组织细胞类型、细胞状态以及免疫细胞状态；能够确定哪些是组织特异性的细胞状态，哪些存在于血液中。通过差异基因表达分析和共变邻域分析（CNA），我们观察到LN病理特征与特定细胞状态显著相关。这些分析揭示了与不可逆慢性组织损伤相关的广泛细胞状态变化。在控制持续组织损伤的影响后，我们发现关键的肾小球巨噬细胞和瘢痕相关巨噬细胞（SAMs）群体的扩增与炎症性疾病活动性的增加同步。SAMs似乎驱动LN纤维化，并且在活动性疾病中比其他髓系细胞更易浸润肾小球。这些观察结果强有力地支持了靶向髓系细胞的治疗策略可能为预防LN肾脏炎症和持续肾损伤提供一种尚未被证实的潜在途径。

## Abstract
One Sentence SummaryA single-cell atlas of paired blood and tissue samples from Lupus Nephritis patients and healthy controls identified stromal and immune populations within renal tissue, including the scar-associated macrophage populations, which correlate with and may drive renal disease activity.

Lupus nephritis (LN), a severe manifestation of Systemic Lupus Erythematosus (SLE), is a heterogeneous disease driven by diverse immune and tissue cell types. We obtained 538K single-cell and 140K single-nuclear profiles from kidney biopsies of 155 LN patients and 30 pre-implantation transplant biopsy controls, along with 325K single-cell blood profiles overlapping many of these patients. We identified key tissue cell types and cell states, and immune cell states; we were able to determine cell states that were tissue specific, and those that were present in the blood. We observed that LN pathological features are significantly associated with cell states using differential gene expression and Covarying Neighborhood Analysis (CNA). These analyses revealed broad changes in cell states associated with irreversible chronic tissue damage. After controlling for the effects of ongoing tissue damage, we observed that expansion of key glomerular and Scar Associated Macrophages (SAMs) populations tracked with increasing inflammatory disease activity. SAMs appear to drive LN fibrosis and, in active disease, infiltrate the glomeruli more than other myeloid cells. These observations strongly support that therapeutic targeting of myeloid populations may offer an as-of-yet unproven strategy to prevent renal inflammation and ongoing kidney damage in LN.

---

## 论文详细总结（自动生成）

好的，作为一名资深学术论文分析助手，我将对这篇题为《狼疮性肾炎血液与组织的群体规模图谱》的预印本论文进行结构化、深入且客观的总结。

---

### **论文结构化总结：A population-scale atlas of blood and tissue in lupus nephritis**

#### **1. 核心问题与整体含义**
*   **研究动机**：狼疮性肾炎（LN）是系统性红斑狼疮（SLE）最严重的并发症之一，具有高度异质性，现有疗法效果不一且副作用大。尽管肾活检是诊断金标准，但其背后的细胞和分子机制仍未完全阐明。先前的研究多局限于血液或小规模组织样本，缺乏大规模、高分辨率的肾脏组织与血液配对分析。
*   **整体含义**：本研究旨在构建一个迄今为止最大规模的LN单细胞图谱，通过整合肾脏组织（单细胞和单核RNA测序）与配对的外周血单核细胞数据，系统性地描绘LN患者肾脏微环境中的免疫细胞和组织细胞的精细状态，并探究这些细胞状态如何与关键的临床病理指标（如活动性指数、慢性化指数）相关联，从而揭示驱动疾病的关键细胞群体和潜在治疗靶点。

#### **2. 方法论**
*   **核心思想**：利用高通量单细胞转录组学技术，对大量LN患者和对照的肾脏活检及血液样本进行无偏倚的细胞普查。通过先进的生物信息学方法整合数据、定义细胞状态，并量化这些状态与临床表型的关联。
*   **关键技术细节**：
    1.  **多模态数据整合**：同时使用单细胞RNA测序（scRNA-seq）和单核RNA测序（snRNA-seq），以克服组织解离过程对不同类型细胞的偏好性影响（如scRNA-seq富集免疫细胞）。使用加权主成分分析和Harmony算法对两种模态的数据进行整合与批次校正。
    2.  **精细细胞状态注释**：在鉴定出8个主要细胞大类后，对每个大类进行亚聚类，最终定义了55个免疫亚群和36个肾实质/基质亚群。
    3.  **组织特异性度量**：通过将肾脏和血液的免疫细胞共同嵌入到一个联合空间中，计算每个细胞的“组织特异性分数”，以区分哪些免疫状态是组织驻留型、血液型或共享型。
    4.  **表型-细胞状态关联分析**：
        *   **共变邻域分析**：采用Covarying Neighborhood Analysis (CNA)方法。该方法不依赖离散的聚类结果，而是在转录组连续空间中定义“邻域”，然后检验每个样本中这些邻域的丰度是否与样本级别的临床变量显著相关。这克服了传统基于聚类频率分析的统计效力限制和多重假设检验问题。
        *   **伪时间轨迹分析**：使用Destiny和Slingshot工具推断B细胞、髓系细胞和T细胞的潜在分化轨迹。
        *   **差异基因表达分析**：基于伪批量数据进行基因水平的关联分析。

#### **3. 实验设计**
*   **数据集/队列**：
    *   **主要队列（AMP SLE cohort）**: 155名活动性LN患者（ISN III, IV, V类）的肾活检样本及匹配的临床病理数据；30名健康活体肾移植供者作为对照。其中118名患者和19名对照有匹配的外周血样本。
    *   **空间转录组验证数据集**: 引用了一个已发表的儿童期发病SLE空间转录组数据集（7例患者+4例对照），用于验证本研究中发现的低丰度免疫细胞的频率是否准确。
*   **Benchmark/对比方法**: 本研究是一项探索性的图谱构建工作，而非方法学比较研究。因此没有设置传统的benchmark或与其他计算方法直接对比。其“金标准”是临床病理指标本身。主要的验证方式包括：
    *   内部验证：比较scRNA-seq和snRNA-seq两种技术下定义的细胞状态及其比例的一致性。
    *   外部验证：将本研究的发现与独立的空间转录组数据进行交叉验证（如B细胞的低丰度）。
    *   生物学合理性验证：发现的关联是否与已知生物学知识一致。

#### **4. 资源与算力**
论文未明确说明具体使用的计算硬件配置（如GPU型号、数量）、软件运行时间或总计算成本。可以推断的是，处理近百万级别的单细胞数据并进行复杂的整合与分析需要相当可观的高性能计算资源。

#### **5. 实验数量与充分性**
实验设计全面且层次分明：
*   **(1) 基础图谱构建**: 对所有样本进行无监督聚类和注释。
*   **(2) 跨组织比较**: 系统分析了肾脏与血液中免疫状态的异同。
*   **(3) 病例-对照分析**: CNA揭示了LN患者相对于健康对照在各类细胞中的显著变化。
*   **(4) LN内部异质性分析 (核心)**:
    *   分别测试了多个临床变量对各类细胞的全局影响。
    *   重点深入分析了两个关键病理指标——慢性化指数和活动性指数——如何驱动特定亚群的改变。这部分进行了大量调整混杂因素的敏感性分析（如调整首次活检状态、招募中心等）。
    *   进一步分析了ISN分型的影响及其与活动性指数的关系。
*   **(5) B/T克隆型分析和受体-配体互作分析**: 探索了B细胞的克隆扩增情况和SAMs与肾小球细胞的潜在相互作用通路。

总体而言，实验数量充足且设计严谨。作者意识到了队列异质性带来的混杂风险（如不同招募中心、是否为首次活检），并在关键关联分析中进行了统计调整。这增强了结论的客观性和可靠性。

#### **6. 主要结论与发现**
1.  **构建了全面的LN单细胞参考图谱**:公开了包含91个精细定义的肾脏及血液免疫/实质/基质亚群的资源库。
2.  **揭示了疾病活动的核心驱动者——瘢痕相关巨噬群**: 
    *   识别出一类表达`GPNMB`、`SPP1`、`FABP5`等标志物的巨噬群簇M5, M7, M9, M11），其转录谱特征类似于在其他器官纤维化中报道的瘢痕相关巨噬群 (SAMs)。
    *   SAMs在肾脏中的比例随疾病活动性指数升高而显著扩增；通过空间数据分析预测并证实SAMs优先浸润于肾小球区域；受体-配体分析提示SAMs可能通过分泌SPP1等因子激活肾小球壁层上皮细胞的EMT通路促进纤维化。
3.  **明确了慢性化损伤的核心特征——近端小管损伤态PT0**: 
    *   一个代表“适应不良修复”的近端小管上皮损伤态PT0的频率随慢性化指数急剧增加。
    *   PT0的比例能解释大部分由慢性化引起的其他类型细胞的改变模式，提示其可作为慢性损伤的良好分子代理指标。
4.  **阐明了病理评分优于传统分型**: 
    在解释肾脏内分子变化方面，“活动性指数”比“ISN分型”更具解释力。例如V类膜性肾病相关的分子变化主要是由于其通常伴随较低的活动性所致。
5.  **指出了外周血的局限性**: 
    尽管外周血能有效区分SLE病例与控制组并显示干扰素信号上调等特征，但其免疫状态的改变无法可靠地反映肾脏内部的疾病活动性或慢性化程度。

#### **7.优点**
1.  ****规模空前****:这是迄今为止最大的LN配对组织和血液的单细胞研究队列之一 ，为领域提供了宝贵的公共资源 。
2. ****技术互补****:结合scRNA-seq和snRNA-seq ，更全面地捕获了对解离敏感的组织驻留型和脆弱的实质/基质/内皮等所有类型 。
3 . ****分析方法先进稳健****:采用CNA这种连续空间分析方法来关联表型和避免离散聚类的偏差 ；同时进行了大量针对混杂因素的统计校正 。
4 . ****从描述到机制线索****:不仅描述了差异存在哪些群体 ，还通过轨迹推断 、空间定位预测 、受体配体互作网络等手段 ，为SAMs等功能提供了初步机制假说 。

####8 .不足局限
1 . ****横断面设计限制因果推断****:所有数据均来自单一时间点活检 ，无法确定观察到的变化是因还是果 。例如无法判断SAMs是驱动炎症还是炎症产物招募而来 。
2 . ****技术局限性导致部分信息丢失****:
      -由于需要解离成单个悬液才能上机测序 ，因此破坏了组织结构信息 。虽然借助外部空间数据进行补充验证但仍属间接证据 。
      -基于droplet平台常规建库方案捕获轻链基因较少限制了B/T克隆型深度解析能力较弱
      -未结合表面蛋白标记物仅凭转录谱定义某些复杂功能亚群可能存在一定模糊性
3 . ****队列异质性挑战****:尽管已尽力校正但纳入患者处于不同治疗阶段用药史各异且来自多个中心这些因素仍可能引入难以完全消除残余混杂效应
4 . ****B淋巴细胞罕见性问题****:研究发现组织中B淋巴细胞比例极低即使比对空间数据也支持此现象非技术假象但这使得针对该重要靶向治疗类别深入探究受限可能需结合淋巴结等其他部位研究

(完)

好的，我将从“不足局限”部分继续，完成对这篇论文的总结。

---

#### **8. 不足与局限**
1.  **横断面设计限制因果推断**：所有数据均来自单一时间点活检，无法确定观察到的变化是因还是果。例如，无法判断SAMs是驱动炎症的元凶，还是炎症发生后被招募至损伤部位的“清道夫”。
2.  **技术局限性导致部分信息丢失**：
    *   由于需要将组织解离成单细胞悬液才能进行测序，因此完全破坏了细胞在原位的空间组织结构信息。虽然作者巧妙地引用了外部空间转录组数据进行补充验证，但这仍是间接证据。
    *   基于droplet平台的常规3‘端或5’端建库方案对B/T细胞受体（BCR/TCR）的捕获效率有限，这限制了对B细胞和T细胞克隆型的深度解析。
    *   未结合表面蛋白标记物（如CITE-seq），仅凭转录谱定义某些复杂的、功能可塑的免疫细胞亚群（如巨噬细胞、T细胞亚型）可能存在一定模糊性。
3.  **队列异质性带来的挑战**：尽管作者在统计分析中尽力校正了混杂因素（如招募中心、是否首次活检），但纳入的患者处于不同的疾病阶段和治疗史（用药各异）。这些临床异质性可能引入难以完全消除的残余混杂效应。
4.  **B淋巴细胞罕见性的问题**：研究发现肾脏组织中的B淋巴细胞比例极低，即使比对空间数据也支持此现象非技术假象。但这使得针对这一重要治疗靶点类别的深入探究受限，可能需要结合淋巴结、骨髓或血液中的B细胞进行更全面的研究。

#### **9. 未来展望**
基于本研究的发现和局限，未来工作可能的方向包括：
1.  **纵向研究与机制验证**：对患者进行纵向采样（如治疗前后多次活检），以追踪SAMs、PT0等关键状态的动态变化，并利用动物模型或体外实验验证其因果作用。
2.  **空间多组学整合**：直接对本研究队列的样本或新样本进行高分辨率空间转录组学（如Visium, Xenium）或多重免疫荧光分析，原位确认SAMs在肾小球区域的定位及其与邻近细胞的相互作用。
3.  **治疗反应预测模型**：利用本图谱构建的精细细胞状态特征，开发基于基线活检样本的分子分型工具，用于预测患者对特定疗法（如抗CD20、抗BAFF等）的治疗反应。
4.  **扩大罕见细胞研究**：采用富集策略或更高深度的测序来深入研究组织驻留B细胞等罕见群体在LN中的作用。

#### **10. 总结评价**
本研究是一项里程碑式的工作。它通过构建大规模、高分辨率的单细胞图谱，将LN的临床病理表型（活动性/慢性化）锚定到了具体的、可重复定义的分子细胞状态上。其核心贡献在于超越了传统的“哪种细胞增多或减少”的描述层面，通过先进的生物信息学方法（如CNA），揭示了驱动疾病活动的核心角色——瘢痕相关巨噬群（SAMs），以及标志慢性化损伤的关键指标——近端小管损伤态（PT0）。这些发现为理解LN的异质性提供了新的框架，并指出了极具潜力的新型治疗靶点和预后生物标志物。尽管存在横断面研究固有的局限性以及技术层面的一些挑战，但本研究产生的丰富数据和资源无疑将为未来LN的基础与转化研究奠定坚实基础。

（完）
