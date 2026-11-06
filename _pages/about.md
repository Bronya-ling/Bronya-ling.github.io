---
layout: blog
title: 关于
hide_title: true
permalink: /about/
redirect_from:
  - /about.html
---
<div class="post-content" markdown="1">
## 致谢

这个网站的搭建参考了 [Pepper 的博客](https://ywpepper.github.io/)。向 Pepper 学习，无限进步！

## 访问统计

<!-- 正式发布后加载独立的关于页计数，本地预览不请求统计服务。 -->
{% if jekyll.environment == 'production' %}
{% assign statistics_url = page.url | absolute_url | url_encode %}
<p><img src="https://hitscounter.dev/api/hit?url={{ statistics_url }}&amp;label=Visits&amp;icon=github&amp;color=%23986640&amp;style=flat" alt="About page visits today and total"></p>
<p class="statistics-note">徽章依次显示今日和累计访问次数，由 <a href="https://hitscounter.dev/">Hits Counter</a> 提供，按本页计数图片的加载次数累计。</p>
{% else %}
<p class="statistics-note">正式发布后，这里将显示关于页的今日和累计访问次数。</p>
{% endif %}
</div>
