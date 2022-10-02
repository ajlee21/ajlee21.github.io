---
permalink: /projects/
layout: archive
title: Projects
research_projects_one:
     - image_path: /assets/images/generic_project.svg
       title: Separating between common and context-specific transcriptional responses
       excerpt: "Distinguishing between common and experiment-specific transcriptional signals using a generative neural network."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/generic-expression-patterns"
          - label: "View preprint"
            icon: "fa-fw far fa-eye"
            url: "https://www.biorxiv.org/content/10.1101/2021.05.24.445440v3.full.pdf"
research_projects_two:
     - image_path: /assets/images/batch_effects_project.svg
       title: Impact of technical variation in large-scale compendia
       excerpt: "Evaluating the effect of technical sources of variability in large-scale gene expression compendia."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/simulate-expression-compendia"
          - label: "View publication"
            icon: "fa-fw far fa-file-alt"
            url: "https://academic.oup.com/gigascience/article/9/11/giaa117/5952607"

research_projects_three:
     - image_path: /assets/images/core_acc_tool.svg
       title: Uncovering nuanced transcriptional patterns in P. aeruginosa compendium
       excerpt: "Investigating the transcriptional patterns of core and accessory gene expression in PAO1 and PA14 strains in a compendium containing thousands of samples from hundreds of distinct experiments."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/core-accessory-interactome"
          - label: "View preprint"
            icon: "fa-fw far fa-eye"
            url: "https://www.biorxiv.org/content/10.1101/2022.04.14.488429v1.full.pdf"

---

## Research Projects

{% include feature_row id="research_projects_one" type="left"%}
{% include feature_row id="research_projects_two" type="right"%}
{% include feature_row id="research_projects_three" type="left"%}
