---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
order: 4
---

<div class="publications-auto" markdown="1">
<a href="https://scholar.google.com/citations?hl=en&user=kv7xdfYAAAAJ&view_op=list_works&sortby=pubdate">
    <img style="height: 20px; float: right;" src="{{ '/assets/img/scholar_logo_64dp.png' | relative_url }}" alt="Google Scholar">
</a>

<br>
{% bibliography -f preprints -q @*[published!=true]* -f papers %}

<sup>*</sup> corresponding author, <sup>†</sup> equal contribution<br>


</div>