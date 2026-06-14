---
layout: about
title: about
permalink: /
subtitle: Theory, Experiment, and Statistical Analysis for Genome Biology and Drug Discovery

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Principal Scientist.</p>
    <p>Genentech, Inc.</p>
    <p>1 DNA Way,</p>
    <p>South San Francisco, CA 94080, USA</p>

news: false # includes a list of news items
latest_posts: false # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

Overview
==============

I am a systems biologist at Genentech's Research & Early Development (gRED), where I combine theory, experiment, and analysis to understand how cells regulate their genomes and to discover drugs that revert disease states to healthy ones. My work pairs top-down observational analysis of complex tissue environments with bottom-up causal perturbations to isolate specific cellular behaviors. By integrating public and in-house datasets, I aim to predict therapeutic efficacy and potential off-target effects across diverse patient contexts.

For my training, I was a Human Frontier Science Program (HFSP) fellow with Alexander van Oudenaarden at the Hubrecht Institute, and completed my PhD at EPFL in computational systems biology advised by Felix Naef.


Research themes
=============

My projects span three approaches — theory, experiment, and statistical analysis — and typically pair two of these at a time (Fig. 1), bringing in both wet and dry lab components to address questions in oncology and genome biology.


<figure>
  <img src="/assets/img/triangle2.png" alt="Three_Approaches" width="300">
  <figcaption><strong>Fig. 1: </strong>Theory, experiment, and statistical analysis for genome biology and drug discovery</figcaption>
</figure>


(1) Theory-driven experimental design
---------------
Theory &harr; Experiment.

Designing informative experiments requires theory: models that predict what can be learned from a given measurement strategy before running it. Rather than experimentally enumerating all possible conditions, we derive theoretical frameworks that quantify information gain, reproducibility limits, and cost-information tradeoffs, then use these to design experiments that maximize signal per dollar.

We have also developed a statistical unmixing method (scChIX-seq) that maps multiple histone modifications in single cells and learns the correlation structure between histone marks ([Yeung\*, Florescu\*, Zeller\* et al 2023](https://www.nature.com/articles/s41587-022-01560-3)).

<figure>
  <img src="/assets/img/scchix_example.png" alt="scchix" width="1000">
  <figcaption><strong>Fig. 2: </strong> Multiplexing and unmixing reveal relationships between chromatin states </figcaption>
</figure>

(2) Statistical analysis of functional genomics technologies
--------------
Experiment &harr; Statistical Analysis.

New functional genomics technologies can measure the regulation and output of every gene across virtually every cell in the body. Making sense of this data requires statistical methods that separate biological signal from technical artifacts in sparse, noisy settings, and that integrate information across experiments performed under vastly different conditions. The goal is inference and prediction that can guide the next experiment or therapeutic hypothesis.

We have shown that combining cell surface markers with histone modification mapping in single cells (sortChIC) can systematically compare genome-wide differences between active (e.g. H3K4me1, H3K4me3) and repressed (e.g. H3K27me3, H3K9me3) chromatin states during blood maturation ([Zeller\*, Yeung\* et al 2022](https://www.nature.com/articles/s41588-022-01260-3)). At Genentech, we extend these approaches to large-scale perturbation screens in oncology, integrating in-house and public datasets to predict therapeutic response across patient contexts.

<figure>
  <img src="/assets/img/sortchic_example.png" alt="sortChIC" width="1000">
  <figcaption><strong>Fig. 3: </strong>Analysis methods that quantify global differences between cell types across chromatin states</figcaption>
</figure>

(3) Principles of genome regulation
---------------
Theory &harr; Statistical Analysis.

Understanding how cells regulate their genomes requires moving from description to mechanism: hypothesizing regulatory principles, articulating them as statistical models, and testing them against carefully crafted null hypotheses. Even well-characterized tissues harbor rich regulatory structure that only becomes visible when the right question is asked of the right data.

We have developed model selection approaches to categorize genes by shared regulatory logic, reducing diverse expression patterns across a tissue to a small number of interpretable principles — for example, quantifying how much tissue-specific dynamics come from individual transcription factors versus cooperation between pairs ([Yeung\*, Mermet\* et al 2018](https://genome.cshlp.org/content/28/2/182.full)), or disentangling sleep-wake driven from circadian processes in gene expression ([Hor\*, Yeung\* et al 2019](https://www.pnas.org/doi/abs/10.1073/pnas.1910590116)). These analyses yield direct predictions testable by experiment, such as CRISPR knockout of enhancers ([Mermet\*, Yeung\* et al 2018](https://genesdev.cshlp.org/content/32/5-6/347.full)), and provide a template for the same regulatory decomposition in disease contexts.


<figure>
  <img src="/assets/img/4cseq_dynamics.gif" alt="4Cseq" width="1000">
  <figcaption><strong>Fig. 4: </strong>Changes in chromatin conformation at Cry1 over 24 hours</figcaption>
</figure>

