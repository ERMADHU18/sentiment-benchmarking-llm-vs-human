# Sentiment Benchmarking: Human vs LLM Analysis

A structured sentiment-analysis project comparing **LLM-generated sentiment patterns** with **human judgments** across **Company A** and **Company B**.

## Overview

This repository contains the analysis notebook and project scaffolding used to generate comparative sentiment charts and statistical summaries.  
The source dataset is **not included** in the repository for confidentiality reasons.

The notebook produces:
- sentiment count comparisons by topic
- sentiment score comparisons by topic
- model-level distribution plots
- human vs. LLM benchmarking charts
- cross-company comparison figures
- statistical similarity and significance analysis

## Confidential data policy

The Excel workbook used in this project is intentionally excluded from version control.

This keeps the repository professional while protecting private research or business data.  
To run the notebook locally, place your workbook in the `data/` folder using the expected filename:

- `data/Full data.xlsx`

That file pattern is already ignored by Git, so it will not be pushed to GitHub accidentally.

## Repository structure

```text
sentiment-benchmarking-llm-vs-human/
├── data/
│   ├── .gitkeep
│   └── README.md
├── docs/
│   └── data_requirements.md
├── notebooks/
│   ├── 01_sentiment_benchmarking_analysis.ipynb
│   └── original_chatgpt_image_and_chart.ipynb
├── outputs/
│   ├── .gitkeep
│   └── README.md
├── .gitignore
├── requirements.txt
└── README.md
```

## Required input workbook

Expected workbook path:
- `data/Full data.xlsx`

Expected worksheet names:
- `Count_CA`
- `Count_CB`
- `Score_CA`
- `Score_CB`

A brief worksheet and column guide is included in `docs/data_requirements.md`.

## Setup

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the notebook:

```bash
jupyter notebook notebooks/01_sentiment_benchmarking_analysis.ipynb
```

## Outputs

Generated figures are saved to the `outputs/` directory, including:
- sentiment count charts
- score comparison charts
- model comparison visuals
- human vs. LLM benchmarking figures
- exported PDF versions of key plots

## Notes

- The notebook includes basic cleanup for common label inconsistencies such as `Postive` → `Positive` and `Netural` → `Neutral`.
- The repository is designed to be shareable **without** exposing raw source data.
- For reproducibility, keep the workbook filename unchanged unless you also update the notebook path references.



