---
permalink: /tools/
layout: archive
title: Tools
tool_one:
	- image_path: #/assets/images/biovectors_screenshot.png
		title: SOPHIE
       	excerpt: "Software to distinguish between common and experiment-specific transcriptional signals."
       	links:
			- label: "View repo"
			  icon: "fab fa-fw fa-github"
              url: "https://github.com/greenelab/sophie"
tool_two:
     - image_path: #https://raw.githubusercontent.com/danich1/annorxiver/65ee4a556ab69f2308e5e4d9192905e8cfec3728/figure_generation/output/Figure_2.png
       title: ponyo
       excerpt: "Software to simulate a compendium-wide gene expression data using a variational autoencoder (VAE)."
       links:
	   		- label: "View repo"
			  icon: "fab fa-fw fa-github"
              url: "https://github.com/greenelab/ponyo"
		    - label: "Pypi"
			  icon: "fa-fw fa-brands fa-python"
			  url: "https://pypi.org/project/ponyo/"

---

## Tools

{% include feature_row id="tool_one" type="left"%}
{% include feature_row id="tool_two" type="right"%}