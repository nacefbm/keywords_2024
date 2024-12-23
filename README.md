# NLP: Keyword Extraction using LLMs and Beyond

## Authors
- **Student:** Nacef Ben Mansour
- **Academic Supervisors:** 
  - Prof. Motassem Al-Rahabi
- **Institution:** Sorbonne University
- **Grade:** 19/20
- **Academic Year:** 2023-2024

## 🎯 Project Context & Vision
This project is part of Sorbonne University's initiative to map and enhance the visibility of research expertise across its laboratories and researchers, supporting the open science movement through improved information accessibility.

## Overview
A comprehensive analysis and implementation of automatic keyword extraction methods, comparing traditional approaches with state-of-the-art Large Language Models using HAL Sorbonne's research publication data.

## 📊 Data Pipeline & Methodology

### 1. Data Collection & Processing
- **HAL API Integration**
  - Custom implementation for accessing HAL Sorbonne's database
  - Systematic data collection methodology

### 2. Data Preparation
- **Database Creation & Cleaning**
  - Language detection and classification
  - Data quality validation
  - Creation of language-specific dataframes
- **Preliminary Analysis**
  - Database structure visualization through flowcharts
  - Data distribution analysis

### 3. Data Storage Optimization
- **Format Analysis & Selection**
  - Evaluation of CSV limitations for complex data
  - Implementation of Parquet format for efficient storage
  - Comparative analysis of storage solutions

### 4. Exploratory Data Analysis
- **Domain Distribution Analysis**
  - Language-specific domain distribution histograms
  - Focus on dominant research domains
- **Keyword Analysis**
  - Language-wise keyword count distribution
  - N-gram size analysis by domain
  - Statistical significance testing

### 5. Keyword Extraction Implementation
- **Algorithms Implemented**
  - Traditional approaches (TextRank, KeyBERT, YAKE!...)
  - LLM integration (Llama3, GPT-4, Claude)
  - Custom implementations

### 6. Performance Evaluation
- **Metrics**
  - F1 score with exact matching
  - Fuzzy matching using Levenshtein distance
  - Cost analysis for LLM usage
  - Novel cost-performance efficiency metric

## 🛠️ Technologies
- **Core Technologies**
  - Python
  - Transformers library
  - OpenAI API
  - Anthropic API
- **Data Processing**
  - Pandas
  - Polars
  - Apache Arrow (Parquet)
  - pke
- **Evaluation**
  - scikit-learn
  - Custom metric implementations

## 📁 Project Structure
```
├── notebooks/
│   └── Keyword_Extraction_HAL.ipynb     # Main implementation notebook
├── data/
│   ├── processed/
│   │   ├── df.parquet                   # Complete dataset
│   │   ├── df_en.parquet               # English subset
│   │   └── df_fr.parquet               # French subset
│   └── results/
│       ├── df_kwbrt.parquet            # BERT results
│       ├── df_kwbrt_title.parquet      # BERT title analysis
│       ├── df_llm.parquet              # LLM results
│       ├── df_llm_title.parquet        # LLM title analysis
│       ├── df_stat.parquet             # Statistical analysis
│       └── df_stat_titre.parquet       # Title statistics
├── docs/
│   ├── Keywords_Presentation.pdf       # Project presentation
│   └── KeywordsPublication.pdf         # Technical documentation
├── visuals/
│   └── sankeymatic_20240218_174859_1900x1200.png  # Flow visualization
└── README.md
```

## 📊 Key Findings
- Distribution patterns in research domains
- Language-specific keyword characteristics
- Performance comparison across extraction methods
- Cost-efficiency analysis of LLM approaches
