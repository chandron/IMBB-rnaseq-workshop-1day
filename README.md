# RNA-seq for Wet-Lab Biologists — Workshop

**IMBB-FORTH Bioinformatics Unit**  
Christos Andronis & Electra Tsaglioti

A 2-hour workshop designed to empower wet-lab researchers who generate RNA-seq data to understand their results and engage confidently with bioinformaticians. Rather than teaching participants to run pipelines themselves, the workshop builds the conceptual vocabulary and practical literacy needed to interpret quality control reports, differential expression outputs, and functional enrichment analyses - so that the data they worked hard to generate becomes a conversation they can fully participate in.

## Workshop dataset

**[GSE96870](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE96870)** — *The effect of upper-respiratory infection on transcriptomic changes in the CNS*

- **Organism:** *Mus musculus* (C57BL/6)
- **Tissue:** Cerebellum
- **Conditions:** Influenza A (PR8 strain, intranasal) vs. non-infected (saline)
- **Platform:** Illumina HiSeq 2500, 100 bp paired-end reads
- **Workshop subset:** Female mice only, Day 0 (non-infected) vs. Day 8 (post-infection), 8 samples total (4 per condition)

## Repository contents

| File | Description |
|---|---|
| `rnaseq_workshop_1day.Rmd` | R Markdown notebook — the main workshop document. Renders to HTML with floating TOC, code folding, and interactive tables. |
| `rnaseq_workshop_1day.html` | The R Markdown notebook's rendered HTML. Either download to open or click [here](https://htmlpreview.github.io/?https://github.com/chandron/IMBB-rnaseq-workshop-1day/blob/main/rnaseq_workshop_1day.html)|
| `InfluenzaAvsNonInfected_edgeR_up.txt` | Upregulated gene list (170 genes, padj < 0.05, \|log2FC\| ≥ 1) |
| `InfluenzaAvsNonInfected_edgeR_down.txt` | Downregulated gene list (103 genes, padj < 0.05, \|log2FC\| ≥ 1) |
| `multiqc_report.html` | multiqc report of raw fastq files. |
| `GSM2545380_1_fastqc.html` | FastQC report from 1 of the raw fastq files. |
| `student_cheatsheet.docx` | Cheatsheet doc with important concepts. |

## Session structure

| Segment | Duration |
|---|---|
| Topic 1 — RNA-seq workflow schematic | 10 min |
| Topic 2 — QC & trimming + MultiQC walkthrough | 25 min |
| Topic 3 — DE pipelines & report interpretation | 15 min |
| Topic 4 — Functional enrichment concepts | 15 min |
| Hands-on — Enrichment analysis with [g:Profiler](https://biit.cs.ut.ee/gprofiler/gost)| 50 min |
| Wrap-up & discussion | 5 min |
| **Total** | **120 min** |

## Prerequisites

No coding experience is required. The workshop uses web-based tools (g:Profiler) for the hands-on activity.

For participants who wish to run the optional R code sections in the notebook:

```r
install.packages(c("tidyverse", "gprofiler2", "DT"))
```

## How to use

1. Clone or download this repository
2. Open `rnaseq_workshop_1day.Rmd` in RStudio
3. Click **Knit** to render the HTML notebook, or follow along with the pre-rendered version provided by the instructors
4. For the hands-on activity, the gene list files (`*_up.txt` and `*_down.txt`) should be in the same directory as the Rmd file

## Scope

⚠️ This workshop covers **eukaryotic** bulk RNA-seq only. Prokaryotic RNA-seq requires different alignment strategies, annotation resources, and analysis tools.

## License

This material is developed by the Bioinformatics Unit, IMBB-FORTH Research Institute, Heraklion, Crete, Greece.

---

*IMBB-FORTH Bioinformatics Unit*
