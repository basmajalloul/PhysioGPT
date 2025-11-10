# PhysioGPT: Ontology-Guided Large Language Model for Multimodal Physiological Reasoning

This repository contains the experimental code, processed results, and validation notebooks 
for the paper **“PhysioGPT: An Ontology-Guided Large Language Model for Interpretable Cognitive 
and Motor Function Assessment.”**

---

## Overview

PhysioGPT is a reasoning framework that integrates **EEG**, **HRV**, and **pose-based gait features**
within an ontology-guided **large language model (LLM)** paradigm.  
It enables transparent, uncertainty-aware assessment of cognitive and motor impairments, 
demonstrating strong cross-domain generalization without retraining.

---

## Repository Structure

├── PhysioGPT_LLM_EEG_HRV.ipynb           # Cognitive–autonomic reasoning experiments (EEG + HRV)
├── PhysioGPT_LLM_POSE.ipynb              # Motor reasoning experiments (pose-based gait data)
├── PhysioGPT_llm_subject_predictions_*.csv  # LLM outputs and classification results
├── eeg_results.csv                       # EEG-based evaluation metrics
├── hrv_results.csv                       # HRV-based evaluation metrics
├── LICENSE
├── README.md

---

## Usage

1. **Run notebooks** in order:
   - `PhysioGPT_LLM_EEG_HRV.ipynb`
   - `PhysioGPT_LLM_POSE.ipynb`

2. Provide an OpenAI API key through environment variable:
   ```python
   from google.colab import userdata
   client = OpenAI(api_key=userdata.get("OPENAI_API_KEY"))
