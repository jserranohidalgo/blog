
---
layout: default
---

<div class="content">
    {{ content }}
</div>

<div class="columns is-multiline">
    {% assign sortedautors = site.authors | sort: "start_date" %}
    {% for author in sortedautors %}
        <div class="column is-12">
            {% include author-media.html %}
        </div>
    {% endfor %}
</div>