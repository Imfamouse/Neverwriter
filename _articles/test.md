---
title: "Тест картинок"
date: 2025-09-24
description: "Тест"
category: "Безопасность"
permalink: /articles/test-md/
---


Проверка вывода Markdown и картинок.

## Вариант 1: обычная Markdown-вставка
![Подпись к изображению]({{ "/assets/img/sms1.jpg" | relative_url }})

## Вариант 2: picture с fallback
<picture>
  <img src='{{ site.assets_path | append: "/sms1.jpg" | relative_url }}'
       alt="Обложка" loading="lazy" width="400" height="200" style="max-width:100%;height:auto">
</picture>

## Вариант 3: figure с подписью
<figure style="text-align:center">
  <img src='{{ site.assets_path | append: "/sms1.jpg" | relative_url }}'
       alt="Схема процесса" loading="lazy" width="1200" height="700"
       style="max-width:100%;height:auto">
  <figcaption>Подпись: кратко что на картинке.</figcaption>
</figure>

