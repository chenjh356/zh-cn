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
&emsp;&emsp;我是[**华大基因生命科学研究院**](https://www.genomics.cn/)的高级研究助理，利用大型语言模型基于微生物组预测人类健康。我在[**中山大学**](https://www.sysu.edu.cn/)有幸在[**钱军教授**]((https://phs.sysu.edu.cn/zh-hans/teacher/510))和华大基因的刘小敏副研究员的指导，完成本科毕业设计，获得了预防医学专业的医学学士学位。之前，我在[**中山大学附属第七医院**](https://www.sysush.com)完成了临床实习。迄今为止，我已发表了7篇研究论文<a href='https://scholar.google.com/citations?user=jqslgHAAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>。

<span style="color: purple;">&emsp;&emsp;我现在正准备攻读博士学位，计划申请计算机科学院或医学院。如果贵研究团队有符合我的背景和研究兴趣的机会，我将非常高兴与您讨论。请随时联系我！</span>

我的研究兴趣和领域包括: 
- 医疗人工智能
- 机器学习和深度学习
- 统计学分析
- 医学影像分析
- 自然语言处理
- 编程


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
<br>申请号:&nbsp;<span>{{pat.appno}}</span>
{%- endif -%}
{%- if pat.authno -%}
&ensp;授权号:&nbsp;<span>{{pat.authno}}</span>
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
<br>&nbsp;登记号:&nbsp;<span>{{software.regno}}</span>
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
- *2023.12* &emsp;BGI龙腾虎跃奖 (布局及优化自动化流程，累计完成超5万样本的自动化交付)
- *2023.01* &emsp;中国健康科普大赛优秀奖 [[作品](/pdf/%E5%88%86%E9%A4%90%E5%88%B6%E7%9A%84%E5%89%8D%E4%B8%96%E4%BB%8A%E7%94%9F.pdf)]&ensp;[[证书](/pdf/%E5%85%A8%E5%9B%BD%E7%A7%91%E6%99%AE%E5%A4%A7%E8%B5%9B.pdf)]
- *2022.09* &emsp;中山大学奖学金.
- *2021.04*  &emsp;美国数学建模大赛一等奖 ([COMAP](https://www.comap.com/)) [[证书](/pdf/2112179.pdf)]
- *2020.06* &emsp;广东省健康科普大赛优秀奖
- *2019.09* &emsp;中山大学奖学金.
- *2016.09* &emsp;宋庆龄奖学金 ([广东省宋庆龄基金会](http://www.gdsclf.org/)).

<span class='anchor' id='conferences'></span>
# 💬&ensp; 学术会议
- *2024.11* &emsp;第十九届国际基因组学大会([ICG-19](https://www.genomics.cn/news/info_itemid_7150.html)), 中国深圳, 参会人和志愿者.
- *2024.06* &emsp;第一届（2024）现代生命科学治理健康学术研讨会, 中国武汉, 荣誉嘉宾.

<span class='anchor' id='teaching'></span>
# <i class="fa fa-chalkboard-teacher"></i>&ensp; 教学授课

- *2024.09* &emsp;**华大教育学院: 宏基因组关联研究的设计和案例分析**. 教学助理, 协助副研究员[刘小敏](https://scholar.google.com/citations?user=rUwI1DkAAAAJ)共同完成授课

<span class='anchor' id='miscellaneous'></span>
# &nbsp;<i class="fa fa-heartbeat" aria-hidden="true" ></i>&ensp; 其他
- 我是擅长多种体育运动。我最喜欢的体育运动是羽毛球。作为华大基因研究院羽毛球队的队长，我带领我的团队在2024年BGI秋季运动会的羽毛球团体比赛中获得冠军! [[新闻](https://mp.weixin.qq.com/s/tOfF7diNTUB2ARJZrjgszg)]
- 编程是我最喜欢的事情之一。我最擅长的编程语言是Python，尤其喜欢编写代码来实现让我们生活更加便利的功能，这给予了我很大的成就感。以下是我的部分作品：
  - [中山大学大学服务中心学生助理管理系统](https://sznc.home.ealeo.xyz:6443/admin)
  - [海南省新冠肺炎患者轨迹文本分析](http://covid-19.infdr.cn/analysis/)
  - [流行病调查轨迹文本结构工具](http://covid-19.infdr.cn/app/)
  - 微信小程序: 中山大学信息技术帮助台
  
