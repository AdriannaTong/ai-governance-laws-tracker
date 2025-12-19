---
title: 中国
---

## 中国AI法律法规

以下内容自动从数据文件中提取，列出中国与人工智能治理相关的法规与政策。

{% for item in site.data.regulations %}
{% if item.country == "中国" %}
### {{ item.title }}（{{ item.year }}）

{{ item.summary_zh }}

- 涉及主题：{{ item.topics | join: ", " }}
- 官方链接：[查看原文]({{ item.official_url }})
- 最近更新：{{ item.last_updated }}

{% endif %}
{% endfor %}
