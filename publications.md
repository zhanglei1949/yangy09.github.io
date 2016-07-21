---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - title: "Missing value imputation for microRNA expression data by using a GO-based similarity measure"
    author: "Yang Yang, Zhuangdi Xu and Dandan Song"
    journal: "BMC bioinformatics"
    volume: "17"
    number: "1"
    pages: "109"
    year: "2016"
    publisher: "BioMed Central"
    
  - title: "Improving clustering of microRNA microarray data by incorporating functional similarity"
    author: "Yang Yang, Zhichen Wu and Wei Kong"
    journal: "Current bioinformatics"
    volume: "in press"
    year: "2016"

  - title: "The Construction of Common and Specific Significance Subnetworks of Alzheimer’s Disease from Multiple Brain Regions"
    author: "Wei Kong, Xiaoyang Mou, Na Zhang, Weiming Zeng, Shasha Li and Yang Yang"
    journal: "BioMed research international"
    volume: "2015"
    year: "2015"
    publisher: "Hindawi Publishing Corporation"
    
  - title: "Roles of small RNAs in soybean defense against Phytophthora sojae infection"
    author: "James Wong, Lei Gao, Yang Yang et al"
    journal: "The Plant Journal"
    volume: "79"
    number: "6"
    pages: "928--940"
    year: "2014"
    publisher: "Wiley Online Library"
    

  - title: "A new feature selection method for computational prediction of type III secreted effectors"
    author: "Yang Yang and Sihui Qi"
    journal: "International journal of data mining and bioinformatics"
    volume: "10"
    number: "4"
    pages: "440--454"
    year: "2014"
    publisher: "Inderscience Publishers Ltd"
    
  - title: "Identification of novel type III effectors using latent Dirichlet allocation"
    author: "Yang, Yang"
    journal: "Computational and mathematical methods in medicine"
    volume: "2012"
    year: "2012"
    publisher: "Hindawi Publishing Corporation"
    
  - title: "Learning from imbalanced data sets with a Min-Max modular support vector machine"
    author: "Bao-Liang Lu, Xiao-Lin Wang, Yang Yang and Hai Zhao"
    journal: "Frontiers of Electrical and Electronic Engineering in China"
    volume: "6"
    number: "1"
    pages: "56--71"
    year: "2011"
    publisher: "Springer"
    
  - title: "Computational prediction of type III secreted proteins from gram-negative bacteria"
    author: "Yang Yang, Jiayuan Zhao, Robyn L Morgan, Wenbo Ma and Tao Jiang"
    journal: "BMC bioinformatics"
    volume: "11"
    number: "1"
    pages: "1"
    year: "2010"
    publisher: "BioMed Central"

  - title: "Protein subcellular multi-localization prediction using a min-max modular support vector machine"
    author: "Yang Yang and Bao-Liang Lu"
    journal: "International Journal of Neural Systems"
    volume: "20"
    number: "01"
    pages: "13--28"
    year: "2010"
    publisher: "World Scientific"
    
  - title: "Computational prediction of novel non-coding RNAs in Arabidopsis thaliana"
    author: "Dandan Song, Yang Yang, Bin Yu, Binglian Zheng, Zhidong Deng, Bao-Liang Lu, Xuemei Chen and Tao Jiang"
    journal: "BMC bioinformatics"
    volume: "10"
    number: "1"
    pages: "1"
    year: "2009"
    publisher: "BioMed Central"
    
  - title: "Feature reduction using a topic model for the prediction of type iii secreted effectors"
    author: "Sihui Qi, Yang Yang and Anjun Song"
    booktitle: "International Conference on Neural Information Processing"
    pages: "155--163"
    year: "2011"
    organization: "Springer"
---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
- {% if pub.url %} [{{pub.title}}]({{pub.url}}).
  {% else %} {{pub.title}}.
  {% endif %}{% if pub.type %}({{pub.type}})
  {% endif %}{{pub.author}}.
  {% if pub.journal %} {{pub.journal}}, {{pub.year}}, {{pub.volume}}({{pub.number}}):{{pub.pages}}
  {% endif %}{% if pub.booktitle %} {{pub.booktitle}}, pp.{{pub.pages}} ({{pub.conference}} {{pub.year}})
  {% endif %}{% if pub.slides %}[Slides]({{pub.slides}}).
  {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
  {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
  {% endif %}
{% endunless %}
{% endfor %}



