---
permalink: /
title: "About"
excerpt: "Miri Krupkin - Structural Biologist & Computational Biophysicist"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Miri Krupkin, Ph.D.
### Structural Biologist & Computational Biophysicist · Stanford University (Puglisi Lab)

I decode the architecture, conformational dynamics, and structural pharmacology of functional RNAs, molecular machines, and ribonucleoprotein (RNP) complexes. My scientific trajectory traces catalytic RNA and ribonucleoprotein assemblies across evolutionary time and macromolecular scale: from the **minimal catalytic proto-ribosome** at the origins of life, to the **intact 2.5-megadalton universal ribosome** targeted by clinical therapeutics, to **massive viral genomic RNAs (>9,000 nt)** whose dynamic conformational transitions orchestrate viral assembly and replication.

To resolve dynamic macromolecular states that resist conventional static structural determination, I integrate high-resolution empirical ground truth (**X-ray crystallography, Cryo-EM/ET, time-resolved 4D synchrotron mechanics, and single-molecule dynamics**) with automated computational validation pipelines, vectorized biophysical analysis, and physics-constrained modeling.

My research foundation spans premier structural biology centers, training directly with Nobel Laureate **Ada Yonath** (Weizmann Institute of Science) and **Elisabetta Viani Puglisi & Joseph Puglisi** (Stanford University), with active consortium collaborations across **SLAC National Accelerator Laboratory, NIH CHEETAH, and the Chan Zuckerberg Biohub**.

[GitHub Profile ↗](https://github.com/mirikrupkin) · [Google Scholar ↗](https://scholar.google.com/citations?user=2U2MWnkAAAAJ&hl=en) · [LinkedIn ↗](https://www.linkedin.com/in/mirikrupkin/) · [PubMed Index ↗](https://pubmed.ncbi.nlm.nih.gov/?term=Krupkin+Miri)

---

## Core Capabilities & Technical Focus

* **Targeting Dynamic RNA Assemblies:** Developing experimental workflows and computational frameworks to isolate, map, and resolve dynamic conformational ensembles in full-length viral genomic RNAs (>9,000 nt), catalytic ribozymes, and viral packaging complexes.
* **Algorithmic Model Validation & Structural QA:** Architecting automated production pipelines to benchmark generative structure predictions (AlphaFold 3, ESMFold) against empirical coordinates, systematically catching hallucination risks, compaction artifacts, and interface misassignments.
* **Structural Pharmacology & Allosteric Mechanisms:** Resolving species-selective drug-binding pockets, allosteric trapping mechanisms, and antibiotic resistance pathways in complex multi-subunit ribosomal machinery.
* **High-Throughput Biophysics & Data Ingestion:** Automated data processing and analytical workflows for macromolecular crystallography, time-resolved 4D synchrotron diffraction, single-molecule fluorescence kinetics, and Cryo-EM.
* **Production Computational Stack:** Vectorized scientific Python (NumPy, SciPy, BioPython), PyTest test-driven development, REST API harvesting (RCSB PDB, EBI AlphaFold DB), and HPC orchestration (Linux/Slurm on Stanford Sherlock).

---

## Featured Software Suites

### [FoldCheck-RNA: Nucleic Acid Structural Integrity Suite ↗](https://github.com/mirikrupkin/foldcheck-rna)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mirikrupkin/foldcheck-rna/blob/main/foldcheck-rna.ipynb)

*Production Python • BioPython • SciPy • RCSB REST API • PyTest*
* **Architecture:** Automated validation pipeline benchmarking generative structure predictions (AlphaFold 3) against empirical Cryo-EM and crystallographic coordinates.
* **Algorithmic Core:** Implements coarse-grained phosphorus (P) backbone alignment to evaluate global topological fold integrity while filtering high-frequency base-stacking noise and crystal contact artifacts.
* **Biophysical Edge Cases:** Features a comprehensive 30+ non-canonical modification registry (pseudouridines, 2'-O-methylations) and automated sequence alignment to benchmark viral RNA domains and circular ribozymes.
* **[View Repository on GitHub ↗](https://github.com/mirikrupkin/foldcheck-rna)**

### [FoldCheck-Pro: Protein Biophysical Validation Suite ↗](https://github.com/mirikrupkin/foldcheck-pro)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mirikrupkin/foldcheck-pro/blob/main/foldcheck-pro.ipynb)

*Production Python • Vectorized NumPy • Hungarian Algorithm • Automated EBI Ingestion*
* **Architecture:** High-throughput pipeline evaluating predicted multimeric protein models against empirical structures to systematically identify hallucinated contacts and interface errors.
* **Algorithmic Core:** Resolves multi-chain heterodimer asymmetry (such as HIV-1 RTase p66/p51) using the Hungarian algorithm (`scipy.optimize.linear_sum_assignment`) for optimal sequence-similarity coordinate assignment.
* **Integrated Biophysics:** Maps Relative Accessible Surface Area (RASA via Shrake-Rupley) against per-residue pLDDT confidence scores to separate stable hydrophobic cores from dynamic surface loops.
* **[View Repository on GitHub ↗](https://github.com/mirikrupkin/foldcheck-pro)**

---

## Research Tracks & Major Scientific Impact

### 1. Dynamics & Packaging of Massive Viral Genomic RNA (Stanford University)
Working with **Professors Joseph Puglisi and Elisabetta Viani Puglisi** in collaboration with the **NIH CHEETAH Consortium** and **Wesley Sundquist (Utah)**:
* Developed biochemical platforms to isolate full-length genomic HIV-1 RNA constructs (>9,000 nt) and dissect conformational switches that govern packaging and reverse transcription initiation.
* Decoded how structural mutations in the 5'UTR leader coordinate viral fitness and drive resistance against frontline therapeutics.
* *Selected Output:* **Krupkin et al.**, *Curr Opin Struct Biol* (2020); Nouhin, ..., **Krupkin et al.**, *J Gen Virol* (2023); Prabhakar, ..., **Krupkin et al.**, *Nucleic Acids Res* (2022).

### 2. Ribosomal Pharmacology & Time-Resolved Dynamics (SLAC & Weizmann Institute)
Investigating structural transitions and antibiotic mechanisms from bacterial pathogens to translation machinery:
* Determined high-resolution crystal structures of bacterial ribosomes complexed with clinical antibiotics (avilamycin, macrolides, pleuromutilins) alongside Nobel Laureate **Ada Yonath**, identifying allosteric rearrangements in proteins uL16 and CTC that block A-site tRNA accommodation.
* Spearheaded 4D time-resolved crystallography workflows with **SLAC National Accelerator Laboratory** capturing transient factor-ribosome intermediate states during translation initiation.
* *Selected Output:* Yapici, ..., **Krupkin et al.**, *(Submitted to EMBO J)*; **Krupkin\* et al.**, *PNAS* (2016); Eyal\*, Matzov\*, **Krupkin et al.**, *PNAS* (2015); Matzov, ..., **Krupkin et al.**, *Nucleic Acids Res* (2017).

### 3. Prebiotic Proto-Ribosomal RNA & Catalytic Machines (Weizmann Institute)
Investigated the evolutionary emergence and structural mechanics of the ribosomal peptidyl transferase center (PTC) with **Professor Ada Yonath**:
* Designed and biochemically validated synthetic proto-ribosomal RNA dimeric constructs capable of spontaneous peptide bond formation independent of ribosomal protein cofactors.
* Modeled active-site conformational geometries and dimerization mechanics using quantum mechanical and computational energy methods.
* *Selected Output:* Bose, ..., **Krupkin et al.**, *Nucleic Acids Res* (2022); Huang, **Krupkin et al.**, *PNAS* (2013); **Krupkin et al.**, *Phil Trans R Soc B* (2011).

---

## High-Impact Publications (Selected)

1. **Krupkin M\***, Wekselman I\*, ..., **Yonath A**. Avilamycin and evernimicin induce structural changes in rProteins uL16 and CTC that enhance the inhibition of A-site tRNA binding. *Proc Natl Acad Sci USA* (2016).
2. Dugan AE, Syangtan D, Nonnecke EB, ..., **Krupkin M**, ..., Ribbeck K, **Xavier RJ**, Bevins CL, **Kiessling LL**. Intelectin-2 is a broad-spectrum antimicrobial lectin. *Nature Communications* 17, 231 (2026).
3. Prabhakar A\*, Krahn N\*, Zhang J\*, ..., **Krupkin M**, ..., **Puglisi EV**, **Söll D**, **Puglisi JD**. Uncovering translation roadblocks during the development of a synthetic tRNA. *Nucleic Acids Res* (2022). **Journal Cover**.
4. Bose T, Fridkin G, Davidovich C, **Krupkin M**, ..., **Yonath A**. Origin of life: proto ribosome forms peptide bonds and links RNA and protein dominated worlds. *Nucleic Acids Res* (2022). *Featured in Nature News*.
5. **Krupkin M\***, Jackson LN\*, Ha B\*, **Puglisi EV**. Advances in understanding the initiation of HIV-1 reverse transcription. *Curr Opin Struct Biol* (2020).
6. Eyal Z\*, Matzov D\*, **Krupkin M**, ..., **Yonath A**. Structural insights into species-specific features of the ribosome from the pathogen *Staphylococcus aureus*. *Proc Natl Acad Sci USA* (2015).

---

<p align="center" style="color: #666; font-size: 0.9em;">
Direct Inquiries: <code>krupkin [at] stanford [dot] edu</code>
</p>
