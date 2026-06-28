# Protein Sequence Transformer (Evo-Biased Sequence Generator)

A lightweight Transformer-based system for generating protein-like amino acid sequences using autoregressive language modeling with an added pairwise interaction bias. Trained specifically on the LuxR family.

The model is trained on bacterial regulatory protein sequences retrieved from UniProt and fallback datasets when online retrieval is unavailable.

This project is an experimental sequence modeling system, not a structural biology or protein folding model.

---

## Check

This system operates purely at the sequence level.

It does NOT model:
- 3D protein structure
- atomic geometry
- residue spatial distances
- folding dynamics
- thermodynamic stability

Any structural plausibility in outputs is incidental, not enforced.

---

## What This Project Actually Is

A hybrid sequence model combining:

- Transformer-based autoregressive language modeling
- Learned pairwise interaction bias between sequence positions
- Heuristic ranking of generated sequences

It is best described as:
> a protein language model with co-occurrence-aware attention bias

---

## Installation

```bash
pip install torch requests numpy matplotlib tqdm certifi urllib3
