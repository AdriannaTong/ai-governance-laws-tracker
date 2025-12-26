---
title: 欧盟
layout: country
---

## 欧盟 AI 法律与政策概览

{% for item in site.data.regulations %}
{% if item.country == "欧盟" %}
### {{ item.title }}（{{ item.year }}）

{{ item.summary_zh }}

- 涉及主题：{{ item.topics | join: ", " }}
- 官方链接：[查看原文]({{ item.official_url }})
- 最近更新：{{ item.last_updated }}

---
{% endif %}
{% endfor %}
