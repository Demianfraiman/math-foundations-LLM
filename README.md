# Why Do Transformers Work?
## A Mathematical Theory via Optimal Transport

This repository contains my undergraduate thesis in Data Science (Universidad de Buenos Aires),
where I develop a **rigorous mathematical framework** to explain why Transformer architectures
are capable of representing complex semantic relationships.

The central idea is to reinterpret **attention mechanisms as entropic optimal transport operators**
acting on probability measures over embedding spaces.

📄 **Full thesis:** [`thesis.pdf`](thesis.pdf)

---

## 🎯 Problem

Modern Transformer-based language models exhibit an impressive ability to capture semantic,
syntactic, and contextual relationships between tokens.  
Despite their empirical success, there is still **no clear mathematical theory** explaining:

- What class of semantic relations Transformers can represent
- Whether attention mechanisms have intrinsic expressive limitations
- In what precise sense Transformers are *universal approximators*

This thesis addresses these questions from a **functional-analytic and measure-theoretic perspective**.

---

## 🧠 Main Idea

Instead of viewing attention as a purely algorithmic operation, the thesis proposes a new viewpoint:

- Texts are modeled as **probability measures** over an embedding space
- Attention matrices are interpreted as **joint probability measures**
- Semantic relations are formalized as **coupling-valued maps**
- Transformers are seen as learning **continuous maps between spaces of measures**

Within this framework, attention becomes a structured instance of **entropic optimal transport**.

---

## 📐 Mathematical Framework

The work combines tools from:

- Real and functional analysis
- Probability theory and weak-* topology
- Optimal transport (classical and entropic)
- Gamma-convergence
- Convex analysis and Banach spaces

In particular, the space of semantic couplings is shown to embed naturally into a Banach space
of continuous functions, allowing approximation arguments.

---

## ⭐ Main Result (Informal)

> **Universal Approximation of Semantic Couplings**  
>  
> Any continuous system of semantic relations between texts—modeled as probability measures—
> can be approximated arbitrarily well by a Transformer architecture whose attention layer
> is implemented via a Sinkhorn (entropic optimal transport) operator.

This provides a **mathematically precise sense** in which Transformers are universal
approximators of semantic structure.

---

## 📘 Thesis Information

- **Title:** Why Do Transformers Work? A Real Analysis Perspective  
- **Author:** Demián Fraiman  
- **Advisor:** Julián Fernández Bonder  
- **Institution:** Universidad de Buenos Aires (FCEN)  
- **Year:** 2025  

---

## 🔭 Why This Matters

This work contributes to the theoretical foundations of deep learning by:

- Explaining attention beyond heuristic or empirical arguments
- Bridging Transformer architectures with optimal transport theory
- Providing a path toward a **mathematical theory of semantic understanding**
- Offering tools potentially relevant to theory tracks (NeurIPS, COLT, ICLR)

---

## 📜 Citation

If you reference this work, please cite:

```bibtex
@mastersthesis{fraiman2025transformers,
  title={Why Do Transformers Work? A Real Analysis Perspective},
  author={Fraiman, Demián},
  year={2025},
  school={Universidad de Buenos Aires}
}
