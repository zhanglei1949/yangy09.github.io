---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "Daniel Haas, Jason Ansel, Lydia Gu, Adam Marcus"
    title: "Argonaut: Macrotask Crowdsourcing for Complex Data Processing"
    keywords: "Locu"
    month: "September"
    year: "2015"
    address: "Kohala Coast, Hawaii"
    booktitle: "International Conference on Very Large Data Bases"
    url: 2015vldb-argonaut.pdf
    bibtex: 2015vldb-argonaut.bib

  - title: "Missing value imputation for microRNA expression data by using a GO-based similarity measure"
    author: "Yang, Yang and Xu, Zhuangdi and Song, Dandan"
    journal: "BMC bioinformatics"
    volume: "17"
    number: "1"
    pages: "109"
    year: "2016"
    publisher: "BioMed Central"
  
  - title: "Roles of small RNAs in soybean defense against Phytophthora sojae infection"
    author: "Wong, James and Gao, Lei and Yang, Yang and Zhai, Jixian and Arikit, Siwaret and Yu, Yu and Duan, Shuyi and Chan, Vicky and Xiong, Qin and Yan, Jun and others"
    journal: "The Plant Journal"
    volume: "79"
    number: "6"
    pages: "928--940"
    year: "2014"
    publisher: "Wiley Online Library"

  - title: "Feature reduction using a topic model for the prediction of type iii secreted effectors"
    author: "Qi, Sihui and Yang, Yang and Song, Anjun"
    booktitle: "International Conference on Neural Information Processing"
    pages: "155--163"
    year: "2011"
    organization: "Springer"
    conference: "ICONIP"
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



