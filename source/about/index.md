---
layout: docs
seo_title: 关于本站
bottom_meta: false
sidebar: []
valine:
placeholder: 有什么想对我说的呢？
---

<center>
{% span large red, Odomu's %}
{% span large yellow, Blog %}
{% p small, 心之所向 素履以往，生如逆旅 一苇以航 %}
</center>
<br>

{% tabs tab-1 %}
<!-- tab <i class="fa fa-bath" aria-hidden="true"></i> 关于我 -->
{% timeline %}
{% timenode 2022-02-01 升级主题 %}
升级博客主题版本到 5.0.0-rc.3
{% endtimenode %}
{% timenode 2022-01-01 博客建立 %}
1. Hexo和Volantis theme 创建博客
2. 博客部署到Github Pages, 并使用netlify加速博客
{% endtimenode %}
{% endtimeline %}
<!-- endtab -->

<!-- tab <i class="fa fa-thermometer" aria-hidden="true"></i> 站点状态 -->
{% radio red checked, 实时监控本站运行状态 %}
<iframe
    src="https://odomu.instatus.com/embed-status/light-md"
    width="230"
    height="61"
    frameBorder="0"
    scrolling="no"
    style="border: none;"></iframe>
<!-- endtab -->
{% endtabs %}
