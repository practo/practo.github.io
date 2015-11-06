---
layout: page
title: Practo
tagline: Engineering blog
---
{% include JB/setup %}

Recent posts

<ul class="posts">
    {% for post in site.posts limit 5 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
        {{ post.content | strip_html | truncatewords:100}}<br>
            <a href="{{ post.url }}">Read more...</a><br><br>
    {% endfor %}
</ul>