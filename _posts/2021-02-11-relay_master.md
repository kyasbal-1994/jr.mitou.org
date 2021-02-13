---
layout: post
title: "リレーマスター"
permalink: /projects/2019/relay_master
---

{% assign pj = site.data.projects | where_exp: "pj", "pj.id == 'relay_master'" | first %}

<img class='top-img lazyload' src='/assets/img/spinner.svg' alt='サムネイル画像' loading='lazy'
{% if pj.thumbnail == "tbu.png" %} data-src='https://img.youtube.com/vi/1ylC6bqWiPg/hqdefault.jpg'
{% else %}                         data-src='/assets/img/thumbnails/2019/relay_master.png'
{% endif %}                        style='margin-bottom: 10px;' />

センサが埋め込まれた特殊なバトンを持って走るだけで，あらゆる運動を解析するシステムを開発しました。データは専用のwebにアップロードして，あなたの運動をAIで分析・最適化します。“リレーマスター” を利用して，プロに匹敵するパフォーマンスを実現してみませんか？

### クリエータ（採択年度：<a href='/projects/2019'>2019年度</a>）
<p>
{% for creator_id in pj.creator_ids %}
  {% include creator.html is_simple=true %}
{% endfor %}
</p>

### メンター
<p>{% include link-to-mentor.html id=pj.mentor_id %}</p>

## 発表動画
<div class="youtube">
  <iframe width="560" height="315" class="lazyload" data-src="https://www.youtube.com/embed/1ylC6bqWiPg?rel=0" frameborder="0" allowfullscreen=""></iframe>
</div>
