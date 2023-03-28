---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
order: 4
---

<div class="publications-auto" markdown="1">

### Papers
[[My Google Scholar profile]](https://scholar.google.com/citations?user=kv7xdfYAAAAJ&hl=en)

{% bibliography -f papers %}

---

### Current preprints
{% bibliography -f preprints -q @*[published!=true]* %}

---

### Conference Abstracts
{% bibliography -f conference_abstracts %}

\* corresponding author<br>
<!-- <strong class="sjrq NA_Q">NQ</strong> not in SJR ranking -->
</div>