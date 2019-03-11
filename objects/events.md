---
title: Liquid objects
description: Liquid objects contain attributes to output dynamic content on the page.
---

Liquid objects contain attributes to output dynamic content on the page.
For example, the product object contains an attribute called title that can be used to output the title of a product.

**Liquid objects** are also often referred to as **Liquid variables**.

To output an object's attribute, wrap the object's name in **{{** and **}}**, as shown below:


<p class="code-label">Input</p>
```liquid
{% raw %}
Anything you put between {% comment %} and {% endcomment %} tags
is turned into a comment.
{% endraw %}
```

<p class="code-label">Output</p>
```liquid
Anything you put between {% comment %} and {% endcomment %} tags
is turned into a comment.
```
 