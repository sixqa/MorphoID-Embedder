# MorphoID: Individual Recognition of Crayfish Across Molting Cycles

[![Paper Status](https://img.shields.io/badge/Paper-Under%20Review-blue)](https://doi.org/placeholder)

## 📌 Overview

MorphoID is a novel biometric identification system designed specifically for crustaceans that overcomes the fundamental challenge of phenotypic reset during molting cycles. Our approach leverages micro-morphological features on the cephalothorax of *Procambarus clarkii* (red swamp crayfish) and a specialized graph neural network architecture to achieve robust individual recognition across multiple molting events.

## 🔬 Research Background

Traditional biometric methods fail for crustaceans due to complete phenotypic reset during periodic molting. Unlike mammals with stable identifiers (fingerprints, iris patterns), crustaceans lack scientifically validated stable biological markers, severely limiting long-term behavioral studies, genetic breeding programs, and population dynamics research. Our work bridges this critical methodological gap.

## 🧠 Technical Approach

Our framework consists of two key components:

1. **Feature Detection**: An enhanced RTMDet-SOSD model precisely locates biological feature points on the cephalothorax region, including spot distribution patterns and micro-protrusions.

2. **Feature Embedding**: The MorphoID-Embedder network, built with our novel **EdgeGATv2Conv** operator, transforms detected points into highly discriminative embeddings by:
   - Combining local geometric modeling with dynamic attention mechanisms
   - Effectively capturing both micro-structural details and macro spatial configurations
   - Maintaining robustness against missing points and acquisition variations

![System Architecture](NA)

## 📊 Key Results

- **98.7% ± 0.8%** rank-1 accuracy across multiple molting cycles
- Equal performance in full-sibling families and non-family groups (genetic independence)
- 72.91 percentage point improvement over baseline EdgeConv approaches
- Robust identification at extremely low false acceptance rates (0.01% FAR → 55.64% TAR)

![Performance Visualization](prefel.png)

## 📁 Repository Status

**Important Notice**: This repository currently contains only project documentation and paper figures. The complete source code, pre-trained models, and dataset processing scripts will be released upon paper acceptance at *Nature Methods*.

## 🗓 Planned Release Contents

Once our manuscript is accepted, this repository will include:

- Full implementation of the MorphoID-Embedder architecture
- Pre-trained models for crayfish individual recognition
- Training and inference scripts with detailed documentation
- Sample datasets and preprocessing pipelines
- Evaluation code for performance metrics and visualizations
- Standardized image acquisition protocol guidelines

## 📚 Citation

If you find our work valuable for your research, please consider citing our paper once published:

```
NA
```

## 🤝 Contact

For research inquiries or collaboration opportunities, please contact:
- **Primary Contact**: [Cheng-long Zhang] ([cheng-long.zhang@outlook.com](mailto:cheng-long.zhang@outlook.com))
- **Lab Website**: [SDAU-AC](NA)

---

*This repository is maintained by the Computational Biology Lab at SDAU-AC. All rights reserved.*
