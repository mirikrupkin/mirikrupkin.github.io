---
permalink: /
title: "About"
excerpt: "Miri Krupkin - Structural Biologist & Computational Scientist"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Miri Krupkin, Ph.D.
### Structural Biologist & Computational Scientist · Stanford University (Puglisi Lab)

I am a structural biologist and biophysicist decoding the architecture, evolution, and conformational dynamics of functional RNAs and ribonucleoprotein complexes. My research traces RNA across biological time and scale: from **proto-ribosomal catalytic RNA machines** at the origins of life, to the **universal ribosome (a 2.5-megadalton RNA/protein engine)** responsible for synthesizing proteins in all living systems, to **massive viral genomic RNAs (>9,000 nt)** whose dynamic conformational states orchestrate the molecular choreography of infection.

To resolve dynamic assemblies that elude static structural determination, I bridge experimental ground truth, including **X-ray crystallography, Cryo-EM/ET, and single-molecule dynamics**, with computational algorithms, physics-constrained modeling, and generative structural validation pipelines.

My academic journey spans international centers of structural biology, training with Nobel Laureate **Ada Yonath** (Weizmann Institute of Science), **Elisabetta Viani Puglisi** (Stanford), and **Joseph Puglisi** (Stanford University).

[GitHub Profile ↗](https://github.com/mirikrupkin) · [Google Scholar ↗](https://scholar.google.com/citations?user=2U2MWnkAAAAJ&hl=en) · [LinkedIn ↗](https://www.linkedin.com/in/mirikrupkin/)

---

## Core Capabilities & Technical Focus

* **Algorithmic Model Validation:** Designing automated suites to detect hallucination risks, compaction errors, and unphysical geometries in AlphaFold and generative structure predictions.
* **Complex Biological Topologies:** Tackling assemblies that challenge predictive models, including massive viral genomic RNAs (>9,000 nt), multi-chain asymmetric heterodimers, and dynamic ribonucleoproteins (RNPs).
* **High-Throughput Biophysics & Data Ingestion:** Automated data pipelines and processing workflows for Cryo-EM / Cryo-ET, single-molecule fluorescence, and macromolecular crystallography.
* **Production Structural Bioinformatics:** Python (NumPy, SciPy, BioPython, py3Dmol), PyTest test-driven development, REST API data harvesting (RCSB PDB, EBI AlphaFold DB), and vectorized coordinate manipulation.
* **Computational Stack:** High-Performance Computing (Linux/Slurm on Stanford Sherlock), vectorized scientific Python, physics-constrained optimization, interactive 3D visualization.

---

## Featured Software Suites & Repositories

### [FoldCheck-RNA: Nucleic Acid Structural Integrity Suite ↗](https://github.com/mirikrupkin/foldcheck-rna)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mirikrupkin/foldcheck-rna/blob/main/foldcheck-rna.ipynb)

*Production Python • BioPython • SciPy • RCSB REST API • PyTest*
* **Architecture:** Automated validation pipeline bridging generative predictions (such as AlphaFold 3) with empirical Cryo-EM and X-ray crystallographic ground truth.
* **Algorithmic Core:** Implements coarse-grained phosphorus (P) backbone superimposition to capture global topological fold geometry while filtering base-stacking noise and crystal packing dimers.
* **Biophysical Edge Cases:** Features a comprehensive 30+ non-canonical modification registry (pseudouridines, 2'-O-methylations) and automated sequence alignment to benchmark viral RNA domains and circular ribozymes.
* **[View Repository on GitHub ↗](https://github.com/mirikrupkin/foldcheck-rna)**

### [FoldCheck-Pro: Protein Biophysical Validation Suite ↗](https://github.com/mirikrupkin/foldcheck-pro)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mirikrupkin/foldcheck-pro/blob/main/foldcheck-pro.ipynb)

*Production Python • Vectorized NumPy • Hungarian Algorithm • Automated EBI Ingestion*
* **Architecture:** High-throughput pipeline evaluating generative protein models against empirical structures to flag hallucination risks and quaternary contact errors.
* **Algorithmic Core:** Resolves multi-chain heterodimer asymmetry (such as HIV-1 RTase p66/p51) using the Hungarian algorithm (`scipy.optimize.linear_sum_assignment`) for optimal sequence-similarity pairing.
* **Integrated Biophysics:** Maps Relative Accessible Surface Area (RASA via Shrake-Rupley) against per-residue pLDDT confidence scores to systematically classify confident hydrophobic cores versus flexible surface loops.
* **[View Repository on GitHub ↗](https://github.com/mirikrupkin/foldcheck-pro)**

---

## Research Tracks & Major Scientific Impact

### 1. Dynamics of Massive Viral Genomic RNA (Stanford University)
Working with **Professors Joseph Puglisi and Elisabetta Viani Puglisi**, I investigate the structural dynamics and regulatory roles of HIV-1 viral RNA during reverse transcription.
* Established experimental and biochemical platforms to isolate full-length viral RNA constructs (>9,000 nt) and dissect conformational transitions across regulatory domains where standard predictive tools break down.
* Decoded how structural mutations in the 5'UTR leader coordinate reverse transcription initiation and drug-resistance adaptations.
* *Key Publications:* **Krupkin et al.**, *Curr Opin Struct Biol* (2020); Nouhin, ..., **Krupkin et al.**, *J Gen Virol* (2023); Prabhakar, ..., **Krupkin et al.**, *Nucleic Acids Res* (2022).

### 2. Ribosomal Antibiotic Resistance & Crystallography (Weizmann Institute)
During my Ph.D. with Nobel Laureate **Ada Yonath**, I determined high-resolution crystal structures of bacterial ribosomes in complex with clinical antibiotics (avilamycin, macrolides, and pleuromutilins).
* Solved the structural mechanism of avilamycin, identifying how allosteric rearrangements in ribosomal proteins uL16 and CTC prevent A-site tRNA accommodation.
* Characterized structural binding pockets of multi-drug resistant pathogens, including *Staphylococcus aureus*, establishing species-specific selectivity mechanisms.
* *Key Publications:* **Krupkin\* et al.**, *PNAS* (2016); Eyal\*, Matzov\*, **Krupkin et al.**, *PNAS* (2015); Eyal\*, Matzov\*, **Krupkin et al.**, *Sci Rep* (2016); Matzov, ..., **Krupkin et al.**, *Nucleic Acids Res* (2017).

### 3. Evolutionary Origins of the Ribosome (Weizmann Institute)
Investigated the prebiotic emergence of the ribosomal peptidyl transferase center (PTC) with **Professor Ada Yonath**.
* Designed and biochemically validated synthetic proto-ribosomal RNA dimeric constructs capable of forming peptide bonds independently of modern ribosomal proteins.
* Modeled RNA structural dimerization and validated active site architectures using quantum chemical and computational methods.
* *Key Publications:* **Krupkin et al.**, *Phil Trans R Soc B* (2011); Bose, ..., **Krupkin et al.**, *Nucleic Acids Res* (2022); Huang, **Krupkin et al.**, *PNAS* (2013).

---

## Selected Publications

1. **Krupkin M**\*, Wekselman I\*, Matzov D, et al. Avilamycin and evernimicin induce structural changes in rProteins uL16 and CTC that enhance the inhibition of A-site tRNA binding. *Proc Natl Acad Sci USA* (2016).
2. Bose T, Fridkin G, Davidovich C, **Krupkin M**, et al. Origin of life: proto ribosome forms peptide bonds and links RNA and protein dominated worlds. *Nucleic Acids Res* (2022).
3. **Krupkin M**\*, Jackson LN\*, Ha B\*, Puglisi EV. Advances in understanding the initiation of HIV-1 reverse transcription. *Curr Opin Struct Biol* (2020).
4. Eyal Z\*, Matzov D\*, **Krupkin M**, et al. Structural insights into species-specific features of the ribosome from the pathogen Staphylococcus aureus. *Proc Natl Acad Sci USA* (2015).
5. Huang L, **Krupkin M**, Bashan A, Yonath A, Massa L. Protoribosome by quantum kernel energy method. *Proc Natl Acad Sci USA* (2013).

---

<p align="center" style="color: #666; font-size: 0.9em;">
Direct Inquiries: <code>krupkin [at] stanford [dot] edu</code>
</p>
