---
permalink: /projects/
layout: archive
title: Projects
research_projects_one:
     - image_path: #/assets/images/biovectors_screenshot.png
       title: Separating between common and context-specific transcriptional responses
       excerpt: "Distinguishing between common and experiment-specific transcriptional signals using a generative neural network."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/generic-expression-patterns"
          - label: "View preprint"
            icon: "fa-solid fa-eye"
            url: "https://www.biorxiv.org/content/10.1101/2021.05.24.445440v3.full.pdf"
research_projects_two:
     - image_path: #https://raw.githubusercontent.com/danich1/annorxiver/65ee4a556ab69f2308e5e4d9192905e8cfec3728/figure_generation/output/Figure_2.png
       title: Impact of technical variation in large-scale compendia
       excerpt: "Evaluating the effect of technical sources of variability in large-scale gene expression compendia."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/simulate-expression-compendia"
          - label: "View publication"
            icon: "far fa-file-alt"
            url: "https://academic.oup.com/gigascience/article/9/11/giaa117/5952607"

research_projects_three:
     - image_path: #https://raw.githubusercontent.com/greenelab/text_mined_hetnet_manuscript/3a040e78114208417d2b1784ae558fb323eabe01/content/images/figures/hetionet/metagraph_highlighted_edges.png
       title: Uncovering nuanced transcriptional patterns in P. aeruginosa compendium
       excerpt: "Investigating the transcriptional patterns of core and accessory gene expression in PAO1 and PA14 strains in a compendium containing thousands of samples from hundreds of distinct experiments."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/core-accessory-interactome"
          - label: "View preprint"
            icon: "fa-solid fa-eye"
            url: "https://www.biorxiv.org/content/10.1101/2022.04.14.488429v1.full.pdf"

---

## Research Projects

{% include feature_row id="research_projects_one" type="left"%}
{% include feature_row id="research_projects_two" type="right"%}
{% include feature_row id="research_projects_three" type="left"%}
