---
layout: default
title: "Архив статей"
---

# 🗂 Архив статей
Добро пожаловать! Здесь собраны разные статьи.

## 📑 Статьи

{% assign sorted_articles = site.articles | sort: 'date' | reverse %}

{% for article in sorted_articles %}
- [{{ article.title }}]({{ article.url | relative_url }})
  {% if article.description %}<br><small>{{ article.description }}</small>{% endif %}
  {% if article.date %}<br><small>📅 {{ article.date | date: "%d.%m.%Y" }}</small>{% endif %}
  {% if article.category %}<br><small>🏷️ {{ article.category }}</small>{% endif %}
{% endfor %}

> Новые статьи будут появляться в этом списке. Следите за обновлениями
