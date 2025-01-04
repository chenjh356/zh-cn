---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# <i class="fa fa-id-card" aria-hidden="true"></i>&ensp; 简介
I am a Senior Research Associate at [**BGI Research**](https://en.genomics.cn/), utilizing large language models to predict health with human microbiome. I earned my Bachelor's degree in Medicine with a specialization in Preventive Medicine from [**Sun Yat-sen University**](https://www.sysu.edu.cn/sysuen/), honored to be advised by  [Prof. Qian Jun](https://phs.sysu.edu.cn/zh-hans/teacher/510). Previously, I completed a clinical internship at [**the Seventh Affiliated Hospital, Sun Yat-sen University**](https://www.sysush.com/en). To date, I have published 7 research papers with <a href='https://scholar.google.com/citations?user=jqslgHAAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>.

<span style="color: purple;">I am now preparing to pursue a PhD, with the intention of enrolling in either the School of Computer Science or the School of Medicine. If your research team has opportunities that align with my background and aspirations, I would be thrilled to discuss. Feel free to contact me!</span>

My research interest includes: 
- AI in Healthcare
- Machine Learning and Deep Learning
- Statistical analysis
- Medical imaging analysis
- Natural Language Processing
- Programming


<!-- # 🎓 Educations 
 -->
<span class='anchor' id='educations'></span>
# <i class="fa fa-graduation-cap" aria-hidden="true"></i>&ensp;教育背景
<div id="Education" class="bio" style="margin-bottom:-15px">
    {% include educations.html %}
</div>

<span class='anchor' id='experiences'></span>
# <i class="fa fa-tasks" aria-hidden="true"></i>&ensp;工作经历
{% include experience.html %}

<span class='anchor' id='publications'></span>
# <i class="fa fa-book" aria-hidden="true" ></i> &ensp;科研论文
{% include publication.html %}

<span class='anchor' id='patents'></span>
# <i class="fa fa-lock" aria-hidden="true" ></i> &ensp;专利
{% for pat in site.patents %}
- &nbsp;
{%- for author in pat.authors -%}
{%- if author == site.author.name or author == site.author.enname -%}
<a href="#" onclick="event.preventDefault()" style="white-space: nowrap;display: inline-block;">`{{ author }}`</a>
{%- else -%}
<a href="#" onclick="event.preventDefault()" style="white-space: nowrap;display: inline-block;">{{ author }}</a>
{%- endif -%}
{%- if forloop.last == false -%},&nbsp;{%- else -%}.&nbsp;{%- endif -%}
{%- endfor %}
**{{pat.title}}**&ensp;
{%- if pat.appno -%}
<br>Application number:&nbsp;<span style="color: red;">({{pat.appno}})</span>
{%- endif -%}
{%- if pat.authno -%}
&ensp;Authorization number:&nbsp;<span style="color: red;">({{pat.authno}})</span>
{%- endif -%}
{%- if pat.html -%}
&emsp;[[HTML]]({{pat.html}})
{%- endif -%}
{%- if pat.pdf -%}
&emsp;[[PDF]]({{pat.pdf}})
{%- endif -%}
{% endfor %}

<span class='anchor' id='softwares'></span>
# <i class="fa fa-cogs" aria-hidden="true" ></i>&ensp;软著
{% for software in site.softwares %}
- &nbsp;
{%- for author in software.authors -%}
{%- if author == site.author.name or author == site.author.enname -%}
<a href="#" onclick="event.preventDefault()" style="white-space: nowrap;display: inline-block;">`{{ author }}`</a>
{%- else -%}
<a href="#" onclick="event.preventDefault()" style="white-space: nowrap;display: inline-block;">{{ author }}</a>
{%- endif -%}
{%- if forloop.last == false -%},&nbsp;{%- else -%}.&nbsp;{%- endif -%}
{%- endfor %}
**{{software.title}}**&ensp;
{%- if software.regno -%}
<br>&nbsp;登记号:&nbsp;<span style="color: red;">{{software.regno}}</span>
{%- endif -%}
{%- if software.html -%}
&emsp;[[HTML]]({{software.html}})
{%- endif -%}
{%- if software.pdf -%}
&emsp;[[PDF]]({{software.pdf}})
{%- endif -%}
{% endfor %}

<span class='anchor' id='honors-and-awards'></span>
# 🏅&ensp; 荣誉奖项
- *2023.12* &emsp;Dragon Soars, Tiger Leaps Award (for deploying and optimizing automation processes, awarded by BGI)
- *2022.09* &emsp;Sun Yat-sen University Scholarship.
- *2021.04*  &emsp;Meritorious Winner of Interdisciplinary Contest In Modeling ([COMAP](https://www.comap.com/)) [[Certificate](pdf/2112179.pdf)]
- *2020.06* &emsp;Excellence Award of Guangdong Health Science Popularization Competition
- *2019.09* &emsp;Sun Yat-sen University Scholarship.
- *2016.09* &emsp;Song Qingling Scholarship ([GUANG DONG SONG QING LING FOUNDATION](http://www.gdsclf.org/)).

<span class='anchor' id='conferences'></span>
# 💬&ensp; 学术会议
- *2024.11* &emsp;The 19th Annual Meeting of the International Conference on Genomics ([ICG-19](https://en.genomics.cn/en-news-278-7053.html)), Shenzhen China, Visitor and Volunteer.
- *2024.06* &emsp;Academic Conference on Modern Life Science-based Health Management, Wuhan China, Honored guest.

<span class='anchor' id='teaching'></span>
# <i class="fa fa-chalkboard-teacher"></i>&ensp; 教学授课

- *2024.09* &emsp;**BGI Cource: Design and case analysis of meta-genome association study**. Teaching Assistant (TA), with A.R. [Xiaomin Liu](https://scholar.google.com/citations?user=rUwI1DkAAAAJ)

<span class='anchor' id='miscellaneous'></span>
# &nbsp;<i class="fa fa-heartbeat" aria-hidden="true" ></i>&ensp; 其他
- I'm an sport nut. I love to play badminton and well master in it. I led my team in the badminton team competition as captain and won the championship at the BGI Fall Games in 2024! [[News](https://mp.weixin.qq.com/s/tOfF7diNTUB2ARJZrjgszg)]
- Programming is one of my favorites. My best programming language is Python, and I especially enjoy writing code to implement features to make our lives easier, which gives me a great sense of accomplishment. Following is my works：
  - [Sun Yat-sen University Student Assistant Management Platform](https://sznc.home.ealeo.xyz:6443/admin)
  - [Analysis of the trajectory of Covid-19 patients in Hainan Province](http://covid-19.infdr.cn/analysis/)
  - [Epidemic Investigation Trajectory Text Structuring Tool](http://covid-19.infdr.cn/app/)
  - WeChat Mini Program: Sun Yat-sen University Information Technology Service Help Desk
  
