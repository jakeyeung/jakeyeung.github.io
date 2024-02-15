---
layout: about
title: about
permalink: /
subtitle: Analytical Methods and Computational Biology

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

I am a computational biologist working at the interface of statistical/machine learning, functional genomics technologies, and genome biology. I focus on understanding how different cells turn/off different parts of our genome to give rise to different functions in our body, and how this control fails in disease.

For my training, I was a Human Frontier Science Program (HFSP) fellow with Alexander van Oudenaarden at the Hubrecht Institute. Before that, I completed my PhD at the EPFL in computational systems biology advised by Felix Naef.


Research themes
=============

My projects span three approaches: computational methods, technology development, and biological function. They often pairs two of these approaches at a time (Fig. 1), bringing in wet and dry lab components.


<figure>
  <img src="/assets/img/triangle2.png" alt="Three_Approaches" width="300">
  <figcaption><strong>Fig. 1: </strong>Blending the three approaches for diagnostics and therapeutics</figcaption>
</figure>


(1) Computationally-driven experimental design
---------------
Computation &harr;technology development.

Inferring new information from single-cell experiments allow us to ask new questions about how cells function. Many wet lab-driven approaches have advanced what we kinds of biological measurements we can make, but trying to experimentally enumerate all possible combinations of measurements or conditions can quickly hit diminishing returns. Developing new statistical methods alongside with new technologies can advance measurement limitations by inferring hidden biological parameters.

Recently, we have recently developed a statistical unmixing method (scChIX-seq) that maps multiple histone modifications in single cells and learns the correlation structure between histone marks ([Yeung\*, Florescu\*, Zeller\* et al 2023](https://www.nature.com/articles/s41587-022-01560-3)). We are building on these multiplexing/unmixing methods to perform large-scale genetic and drug screening.

<figure>
  <img src="/assets/img/scchix_example.png" alt="scchix" width="1000">
  <figcaption><strong>Fig. 2: </strong> Multiplexing and unmixing reveal relationships between chromatin states </figcaption>
</figure>

(2) Principles of data analysis for new functional genomics technologies
--------------
Tech dev &harr; biological function.

<!---
New functional genomics technologies can now measure the regulation and output of every gene in the genome in virtually every cell in the body. However, the analysis side remains the bottleneck because it is unclear what are the most exciting biological questions you can ask from technologies given a specific experiment, and how to craft the analysis to pull out the most relevant information that will inspire the next incisive experiment. Therefore, analyses that go beyond the data exploration stage iterate between bespoke statistical/machine learning models and reasoning about the model outputs in the context of how and why the experiment was performed.
-->

New functional genomics technologies can now measure the regulation and output of every gene in the genome in virtually every cell in the body. However, the analysis side is challenging because it is unclear (a) what are the most exciting biological questions you can ask from different technolgoies given a fixed budget, (b) how to think about the design and analysis to separate biological signal from unwanted technical artifacts in sparse, noisy, and limited data regimes, and (c) how to integrate external information from other experiments done within an institute (with similar equipment, protocols, and staff) and around the world (where many conditions may differ) to improve statistical inference and prediction. 

Recently, we have shown that combining cell surface markers with histone modification mapping in single cells (sortChIC) can systematically compare the genome-wide dfferences between active (e.g. H3K4me1, H3K4me3) and repressed (e.g. H3K27me3, H3K9me3) chromatin states during blood maturation([Zeller\*, Yeung\* et al 2022](https://www.nature.com/articles/s41588-022-01260-3)). We are now developing new ways to infer time information and integrate that in the analysis.

<figure>
  <img src="/assets/img/sortchic_example.png" alt="sortChIC" width="1000">
  <figcaption><strong>Fig. 3: </strong>Analysis methods that quantify global differences between cell types across chromatin states</figcaption>
</figure>

(3) Asking how cells regulate their genomes
---------------
Computation  &harr; biological function.

Although functional genomics technologies can now measure the expression and accessibility of thousands of genes across thousands of cells, discovering regulatory principles that explain the changes in gene expression over time and in different cell types is still challenging. Even when using established technologies, the analysis side remains the bottleneck because one must still refine what are the interesting questions to ask given a specific experiment, and craft the analysis to systematically tackle the question that will inspire the next incisive experiment. Possible principles are hypothesized through data exploration, then articulated in a statistical model, and tested against carefully crafted null hypotheses. At each step one must reason about the outputs in the context of how and why the experiment was performed. 

Recently, we have crafted model selection approaches to systematically categorize genes into a handful of groups that share similar regulation. These methods allow the diverse gene expression patterns in a biological tissue to be explained in terms of a small number of biological regulatory principles, for example quantifying how much tissue-specific dynamics come from individual transcription factors versus cooperation between pairs ([Yeung\*, Mermet\* et al 2018](https://genome.cshlp.org/content/28/2/182.full)) or the contribution of sleep-wake driven versus circadian processes in gene expression dynamics ([Hor\*, Yeung\* et al 2019](https://www.pnas.org/doi/abs/10.1073/pnas.1910590116)). These analyses lead to direct predictions that can be experimentally tested (for example, CRISPR knockout of enhancers [Mermet\*, Yeung\* et al 2018](https://genesdev.cshlp.org/content/32/5-6/347.full)).


<figure>
  <img src="/assets/img/4cseq_dynamics.gif" alt="4Cseq" width="1000">
  <figcaption><strong>Fig. 4: </strong>Changes in chromatin conformation at Cry1 over 24 hours</figcaption>
</figure>

