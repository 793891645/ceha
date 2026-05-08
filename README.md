# ceha
#CEHA: Causal Effect Heterogeneity Atlas
#Methodology
#CEHA quantifies the heterogeneity of CRISPR perturbation effects during cell differentiation by combining trajectory-aware pseudotime binning with NNCI-style nearest-neighbor control matching.
#Code Availability: All analytical scripts and complete source code are deposited at [GitHub repository link].
#Data Source: Norman et al. (2019) K562 Perturb-seq dataset (GEO accession: GSE133344).
#Main Results
#Effect increases along pseudotime: Bin0 < Bin1 < Bin2 (Kruskal–Wallis p = 6.3×10⁻⁶)
#Robustness: A consistent increasing trend was observed across NNCI matching parameters K = 5, 10, and 20
#Effect size: Cohen’s d = 2.14–2.43 (7 genes in total)
#Holdout validation: Correlation between training and holdout sets ρ = 0.895
#Enrichment analysis: Significant enrichment of C/EBP family transcription factors (Fisher’s exact test p = 0.002)
#Limitations
#Single cell line restriction: All analyses were performed in the human chronic myeloid leukemia K562 cell line. Although K562 is widely adopted for hematological disease modeling, its differentiation trajectory may differ from primary hematopoietic cells or other cell line models. Further validation is required to verify the cross-tissue and cross-cell-line #generalizability of the present findings.
#Stringent quality filtering: Only 12 out of 105 perturbed genes passed all QC criteria (≥50 cells per gene, and ≥3 cells in each of at least 2 pseudotime bins). Such strict thresholds ensure high credibility of the results but may exclude certain genes with moderate perturbation effects.
