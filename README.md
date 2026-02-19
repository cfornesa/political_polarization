# Analyzing Hate Speech & Bias Detection Suite

[![Project Status: Active](https://img.shields.io/badge/Project%20Status-Active-success.svg)](https://cfornesa.com/bias-detector)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Deployed on Google Opal](https://img.shields.io/badge/Deployed%20on-Google%20Opal-blue.svg)](https://opal.google/app/1vUJA2IktLVp0KKynli2xPaseY5CzPx-d)

## 🚀 Executive Summary
This repository houses the research, datasets, and cognitive architectures for a **two-phase project** on Hate Speech Detection and Implicit Bias Analysis.

*   **Phase 1 (Research):** A technical capstone using **Random Forest** and **SBERT** models to quantify toxicity and political polarization in social media data.
*   **Phase 2 (Production):** An enterprise-grade **Bias Intelligence System** (Agent) that operationalizes the research into a dual-layer reasoning engine on Google's experimental **Opal** platform.

---

## 🛠️ Live Applications (The "Opal Suite")

| Application | Phase | Architecture | Status | Live Link |
| :--- | :--- | :--- | :--- | :--- |
| **Hate Speech Auditor** | **Phase 1:** Research Demo | **Random Forest Classification** (Trained on DGHS/MLMA) | 🟡 Experimental | [**Launch Auditor**](https://opal.google/app/1mqZU9DRKxT_CkgYDrKbpKXr8LXycPite?results=1GEszd_y70RIfG0GIV85x2-HSkgjNFORu) |
| **Bias Detector** | **Phase 2:** Enterprise Agent | **Dual-Layer Reasoning** (Sentiment Map + Implicit Framework) | 🟢 Active | [**Launch Agent**](https://opal.google/app/1vUJA2IktLVp0KKynli2xPaseY5CzPx-d) |

---

## 🔬 Phase 1: The Hate Speech Auditor (Research Core)
The **Auditor Tool** represents the raw technical findings of the "Analyzing Hate Speech" Capstone. It focuses on **high-velocity classification** of toxic content.

*   **The Problem:** Identifying explicit hate speech and polarization in large-scale political discourse.
*   **The Models:**
    *   **Random Forest:** Utilized for interpretable feature importance (e.g., identifying specific vocabulary linked to hate speech).
    *   **SBERT (Sentence-BERT):** Employed to capture semantic meaning beyond simple keywords, measuring the "toxicity distance" between statements.
*   **The Datasets:** Trained on **DGHS** (Dynamically Generated Hate Speech), **MLMA** (Multi-Label/Multi-Aspect), and **ConvAbuse** datasets.
*   **Key Capability:** This tool provides a probability score for "Toxicity" and "Polarization," designed for researchers analyzing large corpora of text.

---

## 🧠 Phase 2: The Bias Detector (Enterprise Evolution)
The **Bias Detector Agent** evolves the Phase 1 research into a production tool for the workplace. It shifts from simple classification to a **Dual-Process Cognitive Architecture**:

### 1. System 1: The Sentiment Mapping Registry (Fast Path)
*   **Mechanism:** Deterministic lookup against a curated **High-Velocity Toxicity Registry** derived from the Phase 1 datasets.
*   **Purpose:** Instant identification of explicit hate speech, slurs, and violent rhetoric with zero latency.
*   **Source Data:** See `Sentiment_Mapping_Table.csv`.

### 2. System 2: The Implicit Bias Framework (Slow Path)
*   **Mechanism:** A "Counterfactual Inference Engine" (The Flip Test). The agent mentally swaps demographic markers (e.g., changing "she" to "he") to detect tonal discrepancies and double standards.
*   **Purpose:** Catches subtle, institutional bias—like gendered performance reviews or ageist job descriptions—that standard filters miss.
*   **Validation:** Grounded in the **Implicit Bias Framework** (see `Bias_Framework.pdf`).

---

## 📂 Repository Structure

```text
├── 📁 datasets/
│   ├── dghs_sa_punc_imbalanced.csv       # Dynamically Generated Hate Speech Dataset
│   ├── mlma_hate_speech_sa_punc_imbalanced.csv # Multi-Label/Multi-Aspect Hate Speech
│   └── convabuse_sa_punc_imbalanced.csv  # Conversational Abuse Dataset
│
├── 📁 notebooks/
│   ├── 01_EDA_and_Preprocessing.ipynb    # Data cleaning & imbalance handling
│   ├── 02_Model_Training_RandomForest.ipynb # Baseline model training (Auditor Logic)
│   └── 03_SBERT_FineTuning.ipynb         # Semantic search implementation
│
├── 📁 architecture/
│   ├── Bias_Framework.pdf                # The definitions used for "System 2" reasoning
│   ├── Sentiment_Mapping_Table.csv       # The registry used for "System 1" filtering
│   └── Fornesa_Christopher_Capstone.pdf  # The original academic research paper
│
└── README.md
```

## 🔗 Connect with the Creator

*   **Portfolio (Capstone):** [Analyzing Hate Speech](https://cfornesa.com/analyzing-hate-speech)
*   **Portfolio (Tool):** [Bias Detector Agent](https://cfornesa.com/bias-detector)
*   **LinkedIn:** [Christopher Fornesa](https://www.linkedin.com/in/christopher-fornesa/)

---

### **Citation**

If you use this research or methodology, please cite:

> **Fornesa, C. (2025).** *Analyzing Hate Speech: From Random Forest Classification to Agentic Bias Detection.* Boston University MSDS Capstone.
