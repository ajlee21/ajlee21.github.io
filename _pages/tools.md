---
permalink: /tools/
layout: archive
title: Tools
tool_one:
     - image_path: /assets/images/sophie_tool.png
       title: SOPHIE
       excerpt: "Software to distinguish between common and experiment-specific transcriptional signals."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/sophie"
tool_two:
     - image_path: /assets/images/ponyo_tool.png
       title: ponyo
       excerpt: "Software to simulate a compendium-wide gene expression data using a variational autoencoder (VAE)."
       links:
          - label: "View repo"
            icon: "fab fa-fw fa-github"
            url: "https://github.com/greenelab/ponyo"
          - label: "Pypi"
            icon: "fab fa-fw fa-python"
            url: "https://pypi.org/project/ponyo/"

---

## Tools

{% include feature_row id="tool_one" type="left"%}
{% include feature_row id="tool_two" type="right"%}