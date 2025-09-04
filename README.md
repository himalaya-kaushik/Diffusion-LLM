# Hybrid Translation Model (Diffusion + Autoregressive)

**Type:** Proof of Concept (Research Notebook)  

This project explores a **hybrid translation framework** inspired by Apple’s *ML-Planner*.  
It combines a **diffusion-based semantic planner** with an **autoregressive decoder**, enabling more coherent and grammatically sound translations, especially for **low-resource languages**.  

---

##  Problem Motivation
- Traditional sequence-to-sequence models often struggle with **long-range context** and **structural coherence**.  
- Low-resource languages like Bengali lack sufficient high-quality parallel data.  
- Purely autoregressive models generate fluent but sometimes semantically inconsistent translations.  

---

##  Approach
1. **Diffusion-Based Planner**  
   - Generates a **global semantic plan** of the target sentence.  
   - Captures long-range dependencies and structural alignment.  

2. **Autoregressive Decoder**  
   - Refines the plan into fluent, token-level translations.  
   - Ensures natural grammar and idiomatic correctness.  

3. **Integration with IndicNLP**  
   - Adapted the pipeline for **English → Bengali** translation.  
   - Helps address low-resource translation challenges by leveraging IndicNLP tokenizers & preprocessing.  

---

##  Key Highlights
- **Hybrid Architecture** → Planner ensures global coherence, decoder ensures local fluency.  
- **Improved Metrics** → Outperformed single-model baselines with higher **BLEU** and **chrF++** scores.  
- **Semantic Fidelity** → Better preservation of meaning and nuance, particularly in complex sentences.  
- **Low-Resource Friendly** → Demonstrated strong results for **English → Bengali** translation.  

---

##  Results
- **BLEU & chrF++**: Significant improvements over autoregressive-only and diffusion-only baselines.  
- **Qualitative Gains**:  
  - Improved sentence-level coherence.  
  - More natural grammar and syntax.  
  - Reduced semantic drift in long sentences.  

---

##  Status
This project is a **Proof of Concept (POC)** implemented in a Jupyter notebook.  
It is not a production-ready system, but serves as a strong demonstration of hybrid translation potential.  

---


