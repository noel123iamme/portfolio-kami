---
layout: post
title: Blogs
---
<div class="posts">
  <ul>
    {% for post in site.posts %}
    <li class="post-teaser">
      <header>
        <h3>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
            {{ post.title }}
          </a>
        </h3>
        <p class="meta">
          {{ post.date | date: "%B %-d, %Y" }}
        </p>
      </header>
      <div class="excerpt">
        {{ post.excerpt | | strip_html | strip_newlines | truncate: 120 }}
      </div>
      <a href="{{ post.url | prepend: site.baseurl }}">
        {{ site.theme.str_continue_reading }}
      </a>
    </li>
    {% endfor %}
  </ul>
</div>

{% if paginator.total_pages > 1 %}
<div class="pagination">
  {% if paginator.previous_page %}
  <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}" class="button" >
    <i class="fa fa-chevron-left"></i>
    {{ site.theme.str_prev }}
  </a>
  {% endif %}
  {% if paginator.next_page %}
  <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}" class="button" >
    {{ site.theme.str_next }}
    <i class="fa fa-chevron-right"></i>
  </a>
  {% endif %}
</div>
{% endif %}

