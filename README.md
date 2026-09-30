# From Genome to Cell: Exploring FGFR3 Using the UCSC Cell Browser

**Name:** Jerrick Paul T. Tayos  
**Assigned Gene:** FGFR3  
**Associated Disease:** Achondroplasia / Skeletal Dysplasias  
**Date:** September 30, 2026  

## UCSC Cell Browser Activity

This activity investigates the expression of the human **FGFR3** gene at the single-cell level using the **UCSC Cell Browser**. The activity focuses on exploring a relevant human tissue dataset, examining cell clusters and cell types, visualizing FGFR3 expression, and comparing its expression with marker genes.

## Assigned Gene and Disease

The assigned gene is **FGFR3 (Fibroblast Growth Factor Receptor 3)**, and the associated disease is **Achondroplasia** (and other skeletal dysplasias).

The FGFR3 gene is relevant to this activity because pathogenic variants in FGFR3 lead to overactivation of the receptor, which negatively regulates bone growth and skeletal development, resulting in dwarfism and related skeletal dysplasias.

## Organ/Tissue Choice and Dataset Information

### Relevant Organ/Tissue

Skeletal muscle and connective/skeletal tissue were selected because FGFR3 functions in regulating fibroblast growth factor signaling in progenitor and mesenchymal cell populations within the musculoskeletal system.

### Selected Dataset

**Dataset Name:** Muscle Cell Atlas  

**Organ/Tissue:** Human Skeletal Muscle  

**Organism:** Homo sapiens  

**Number of Cells:** 22,058 cells  

**Dataset URL:**[ https://cells.ucsc.edu/?ds=muscle-cell-atlas  ](https://cells.ucsc.edu/?ds=muscle-cell-atlas)

### Why This Dataset Was Selected

The Muscle Cell Atlas dataset was selected because skeletal muscle contains diverse musculoskeletal cell lineages—including muscle stem cells (MuSCs), progenitors, fibroblasts, and smooth muscle cells—allowing the expression of FGFR3 to be examined across progenitor and structural cell populations in human skeletal tissue.

<img width="1365" height="767" alt="Screenshot 2026-09-30 081800" src="https://github.com/user-attachments/assets/94cdc66e-24b5-4f36-bf37-1f2faf6c1ed2" />

**Figure 1. Selected Muscle Cell Atlas dataset.**

## Understanding the Cell Map

### Visualization Type

The dataset is displayed using a **UMAP (Uniform Manifold Approximation and Projection)** visualization. UMAP reduces high-dimensional single-cell expression data into a two-dimensional map so that cells with more similar molecular profiles are generally positioned closer together.

### Meaning of Each Dot

Each dot represents one measured **single cell** (or nucleus) in the dataset. The Muscle Cell Atlas dataset contains approximately **22,058 cells**.

### Meaning of the Clusters

The clusters represent different **muscle cell types or progenitor cell populations** identified in the Muscle Cell Atlas dataset. Cells within the same cluster have similar overall transcriptomic profiles, while the different clusters represent distinct cell lineages or functional states within skeletal muscle tissue.

## Expression Plot

### Selected Cell Population / Comparison
Dot plot analysis comparing gene expression across all identified cell clusters in the Muscle Cell Atlas dataset.

### Expression Level Compared to Background
The dot plot demonstrates that dataset-wide marker and dataset genes vary significantly in intensity (dot color) and percentage of expressing cells (dot size). For *FGFR3*, expression remains extremely sparse across all clusters compared to highly expressed structural or lineage-specific markers like *HBA2* in erythroblasts or *COL1A2* in fibroblasts.

### Insights From the Expression Plot
While the 2D UMAP scatter plot displays cell positioning, the dot plot provides quantitative metrics on both expression magnitude (average expression per cell) and population prevalence (fraction of non-zero expressing cells). It confirms that most cells in skeletal muscle display low or zero *FGFR3* transcript detection under standard single-cell RNA sequencing thresholds.

<img width="1365" height="767" alt="Screenshot 2026-09-30 084637" src="https://github.com/user-attachments/assets/f0c6437a-49f8-487e-98dd-32da8324afbf" />
**Figure 4. Dot plot expression comparison across Muscle Cell Atlas clusters.**

---

## Marker Genes

### Cluster Examined
**MuSCs and progenitors 1** (Muscle Stem Cells)

### Marker Genes Listed in Dataset
1. **MYBPC1** (Myosin Binding Protein C1)
2. **IGFBP7** (Insulin Like Growth Factor Binding Protein 7)
3. **COL1A2** (Collagen Type I Alpha 2 Chain)

### Does FGFR3 Act as a Cell-Type Marker?
No, **FGFR3** does not behave as a cell-type marker in this dataset. A marker gene uniquely and strongly identifies a specific cell lineage with a high percentage of non-zero cells (large dot size). In contrast, FGFR3 exhibits low frequency and sparse detection, reflecting its specialized receptor/signaling role rather than a lineage-defining cell identity marker.

<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/7e94aba8-8241-4037-aabc-c8c9a6c44a5e" />
**Figure 5. Cluster marker gene expression table across dataset clusters.**

---

## Disease Gene vs. Marker Gene

* **Assigned Disease Gene:** FGFR3
* **Marker Gene Examined:** COL1A2 (or IGFBP7)

### Comparison of Patterns
* **Which gene shows a more cell-type-restricted expression pattern?**
  Marker genes like **COL1A2** or **MYBPC1** show high expression restricted strictly to their corresponding lineages (e.g., *COL1A2* in Fibroblasts, *MYBPC1* in Myonuclei).
* **Which gene appears more broadly expressed or sparse?**
  **FGFR3** appears extremely sparse with low overall detection levels across adult muscle cell clusters.

### Biological Insight
A **cell-type marker gene** defines structural or lineage identity and is expressed uniformly at high levels in specific cells. A **disease-associated receptor gene** like *FGFR3* mediates precise cellular signaling (particularly during bone and skeletal development), meaning its clinical importance does not require it to be highly abundant or act as a cell-type marker in adult tissues.

## Connection to Genome Browser and ClinVar

### 1. Chromosomal Location
**FGFR3** is located on **Chromosome 4p16.3** (human genome build GRCh38/hg38).

### 2. Disease-Associated Variant Examined Previously
The canonical pathogenic variant associated with Achondroplasia is **c.1138G>A (p.Gly380Arg)** in *FGFR3*, which causes a constitutive gain-of-function activation of the receptor.

### 3. Cell Types Expressing the Gene
In the Cell Browser dataset, low/sparse expression is observed primarily in progenitor and mesenchymal lineages (**MuSCs and progenitors**, **Endothelial cells**, and **Smooth muscle cells**).

### 4. Biological Connection (3–5 Sentences)
*FGFR3* encodes a transmembrane receptor tyrosine kinase that negatively regulates chondrocyte proliferation and bone elongation during endochondral ossification. In embryonic and developing skeletal tissues, mutant FGFR3 leads to premature differentiation of growth plate chondrocytes, resulting in shortened long bones and dwarfism. In adult skeletal muscle, its low expression in progenitor cells reflects its restricted signaling role in quiescent or repairing tissue rather than in mature contractile fibers.

### 5. Can a Single Cell Browser Dataset Prove Causality?
No, a single-cell dataset cannot prove that a gene causes a disease. Single-cell RNA sequencing shows observational correlations in transcript abundance within measured tissues, but proving genetic causality requires functional validation experiments, animal knockout/knock-in models, and genetic association studies (such as ClinVar variants and pedigree analyses).

---

## Reflection

1. **What did the UCSC Cell Browser show that the UCSC Genome Browser could not?**  
   The UCSC Genome Browser displays linear genomic structure, gene annotations, sequence variants, and DNA-level alignment. In contrast, the UCSC Cell Browser reveals cell-type-specific transcriptomic expression profiles, allowing us to see which specific cell populations express the gene at single-cell resolution.

2. **Why can the same gene have different expression levels among different cell types?**  
   Cellular differentiation drives distinct gene regulatory networks, epigenetic modifications, transcription factor availability, and promoter accessibility, leading to highly specific cell-type expression profiles adapted for specific tissue functions.

3. **Why should you be careful when interpreting a gene that shows zero or very low expression in single-cell data?**  
   Single-cell RNA sequencing suffers from technical limitations, including gene "dropouts" caused by low mRNA capture efficiency, transient transcriptional bursting, or the dataset representing mature adult tissue rather than the embryonic developmental window where the gene is most active.

4. **Why is it useful to combine information about genomic location, genetic variants, and cell-specific gene expression?**  
   Integrating genomic locus data, pathogenic variant mechanisms, and single-cell expression profiles bridges genotype to phenotype. It reveals where in the body and at what cellular stage a genetic defect manifests to cause disease.

5. **What was the most interesting observation you made about your assigned gene?**  
   The most interesting observation was discovering that although *FGFR3* mutations cause severe structural skeletal dysplasias, its transcript levels in adult tissue datasets are remarkably low (0.3% frequency), underscoring that receptor signaling genes often operate at low abundance or during narrow developmental windows.

---

## References and Links

* UCSC Cell Browser: https://cells.ucsc.edu/
* Muscle Cell Atlas Dataset: https://cells.ucsc.edu/?ds=muscle-cell-atlas
* UCSC Genome Browser: https://genome.ucsc.edu/
* NCBI ClinVar: https://www.ncbi.nlm.nih.gov/clinvar/
