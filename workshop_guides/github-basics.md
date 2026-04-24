# GitHub Basics
## IMBB Data Analysis Course

This page explains just enough about GitHub to navigate the course repositories.

---

## What is GitHub?

GitHub is a website where code and files are stored and shared. Think of it as Google Drive for code. The course materials live in **repositories** (or "repos") — folders that contain all the files for each part of the course.

For example, some course repositories are:

👉 **Week 1** — [https://github.com/cgenomicslab/imbb-data-analysis](https://github.com/cgenomicslab/imbb-data-analysis)

👉 **Week 2 – RNA-seq session** — [https://github.com/chandron/IMBB-rnaseq-workshop-1day](https://github.com/chandron/IMBB-rnaseq-workshop-1day)


---

## Navigating a repository

When you open a repository page, you will see a list of folders and files. Click any folder to open it and see what's inside, just like browsing folders on your computer.

For example, the Week 1 repository looks like this:

```
imbb-data-analysis/
├── week1/        ← notebooks for Week 1
├── precourse/    ← preparation notebooks
├── data/         ← datasets
└── docs/         ← setup instructions
```

And the RNA-seq session repository looks like this:

```
IMBB-rnaseq-workshop-1day/
├── workshop_materials/
│   ├── rnaseq_workshop_1day.Rmd     ← main workshop document (R Markdown - must be "Knit" in Rstudio, or you can use the rendered version)
│   ├── rnaseq_workshop_1day.html    ← rendered version — download to view
│   ├── GSM2545380_1_fastqc.html     ← FastQC report — download to view
│   ├── multiqc_report.html          ← MultiQC report — download to view
│   ├── SARTools_report.html         ← SARTools report — download to view
│   ├── student_cheatsheet.docx      ← A Cheatsheet of important concepts — download to view
│   ├── InfluenzaAvsNonInfected_edgeR_up.txt
│   └── InfluenzaAvsNonInfected_edgeR_down.txt
├── workshop_guides/
│   ├── rstudio-installation.md
│   └── github-basics.md             ← you are here!
├── LICENSE
└── README.md
```

Click a folder or file name to open it. Use the folder path at the top (called a "breadcrumb") to navigate back.

---

## Previewing files on GitHub

When you click on a file, GitHub shows you a preview. What you see depends on the file type:

| File type | What you see on GitHub | Example in this course |
|---|---|---|
| `.md` (Markdown) | ✅ Rendered — looks like a normal formatted page | `README.md`, `rstudio-installation.md` |
| `.ipynb` (Jupyter notebook) | ✅ Rendered — shows the notebook with outputs | Week 1 notebooks |
| `.txt` | ✅ Plain text — readable as-is | `InfluenzaAvsNonInfected_edgeR_up.txt` |
| `.html` | ⚠️ **Raw HTML code** — not a rendered page | `rnaseq_workshop_1day.html` |
| `.rmd` (R Markdown) | ⚠️ **Raw code** — not a rendered page | `rnaseq_workshop_1day.Rmd` |
| `.docx` (Word document) | ⚠️ **Not readable** — shows as garbled text | `student_cheatsheet.docx` |

> ⚠️ **Important:** `.html`, `.rmd`, and `.docx` files do not display properly on GitHub. `.html` and `.rmd` show as raw code; `.docx` shows as garbled text. To view any of these properly, you need to **download them first** and open them on your computer (see below).

---

## Downloading files

### Download a single file

1. Click on the file you want to download
2. Look for the **download icon** (⬇) in the top-right corner of the file preview and click it
3. The file will be saved to your Downloads folder

Then open it normally — `.html` files open in your browser, `.docx` files open in Word.

### Download everything at once

To get all materials from a repository in one go:

1. Go to the main repository page
2. Click the green **Code** button (top-right of the file list)
3. Select **Download ZIP**
4. Extract the ZIP file somewhere convenient (e.g., Desktop or Documents)

---

## When files get updated

The instructors may add or update files during the course. If you downloaded the ZIP at the start, you won't get these updates automatically.

The simplest fix: **download the ZIP again** and replace the old folder. As long as you save your own work under a different filename, nothing will be lost.

---

## 🎉 That's it

You don't need to know anything else about Git or GitHub for this course.
