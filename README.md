# Analyzing Hate Speech & Bias Detection Suite

[![Project Status: Active](https://img.shields.io/badge/Project%20Status-Active-success.svg)](https://cfornesa.com/bias-detector)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Deployed on Google Opal](https://img.shields.io/badge/Deployed%20on-Google%20Opal-blue.svg)](https://opal.google/app/1vUJA2IktLVp0KKynli2xPaseY5CzPx-d)

## 🚀 Executive Summary
This repository houses the research, datasets, and cognitive architectures for a two-phase project on **Hate Speech Detection** and **Implicit Bias Analysis**.

What began as an academic capstone using **Random Forest** and **SBERT** models to classify political toxicity has evolved into a production-grade **Bias Intelligence System** deployed on Google's experimental **Opal** platform.

---

## 🛠️ Live Applications (The "Opal Suite")

| Application | Type | Architecture | Status | Live Link |
| :--- | :--- | :--- | :--- | :--- |
| **Bias Detector** | Enterprise Agent | **Dual-Layer Reasoning** (Sentiment Map + Implicit Framework) | 🟢 Active | [**Launch App**](https://opal.google/app/1vUJA2IktLVp0KKynli2xPaseY5CzPx-d) |
| **Hate Speech Auditor** | Research Demo | **Random Forest Classification** (Trained on DGHS/MLMA) | 🟡 Experimental | [**Launch App**](https://opal.google/app/1mqZU9DRKxT_CkgYDrKbpKXr8LXycPite?results=1GEszd_y70RIfG0GIV85x2-HSkgjNFORu) |

---

## 🧠 The Dual-Layer Methodology

The core innovation of this project is the shift from simple keyword filtering to a **Dual-Process Cognitive Architecture**:

### 1. System 1: The Sentiment Mapping Registry (Fast Path)
*   **Mechanism:** Deterministic lookup against a curated **High-Velocity Toxicity Registry** derived from the MLMA and DGHS datasets.
*   **Purpose:** Instant identification of explicit hate speech, slurs, and violent rhetoric with zero latency.
*   **Source Data:** See `dghs_sa_punc_imbalanced.csv` and `mlma_hate_speech_sa_punc_imbalanced.csv`.

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
│   ├── 02_Model_Training_RandomForest.ipynb # Baseline model training
│   └── 03_SBERT_FineTuning.ipynb         # Semantic search implementation
│
├── 📁 architecture/
│   ├── Bias_Framework.pdf                # The definitions used for "System 2" reasoning
│   ├── Sentiment_Mapping_Table.csv       # The registry used for "System 1" filtering
│   └── Fornesa_Christopher_Capstone.pdf  # The original academic research paper
│
└── README.md

## 🔗 Connect with the Creator

*   **Portfolio (Capstone):** [Analyzing Hate Speech](https://cfornesa.com/analyzing-hate-speech)
*   **Portfolio (Tool):** [Bias Detector Agent](https://cfornesa.com/bias-detector)
*   **LinkedIn:** [Christopher Fornesa](https://www.linkedin.com/in/christopher-fornesa/)

---

### **Citation**

If you use this research or methodology, please cite:

> **Fornesa, C. (2025).** *Analyzing Hate Speech: From Random Forest Classification to Agentic Bias Detection.* Boston University MSDS Capstone.
