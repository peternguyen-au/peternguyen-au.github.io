---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Welcome to my blog! Here I share my thoughts on software engineering, technology, and problem-solving.

---

<div class="blog-list">
{% for post in site.posts %}
  <article class="blog-post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
      {% if post.author %} • {{ post.author }}{% endif %}
      {% if post.tags %}
        <span class="tags">
          {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>
          {% endfor %}
        </span>
      {% endif %}
    </p>
    <div class="post-excerpt">
      {{ post.excerpt }}
    </div>
    <a href="{{ post.url }}" class="read-more">Read more →</a>
  </article>
  <hr>
{% endfor %}
</div>

{% if site.posts.size == 0 %}
<div class="no-posts">
  <p>No posts yet. Check back soon!</p>
</div>
{% endif %}

<style>
.blog-list {
  max-width: 800px;
  margin: 0 auto;
}

.blog-post {
  margin-bottom: 40px;
}

.blog-post h2 {
  margin-bottom: 10px;
}

.blog-post h2 a {
  text-decoration: none;
  color: inherit;
}

.blog-post h2 a:hover {
  color: #155799;
}

.post-meta {
  color: #666;
  font-size: 0.9em;
  margin: 10px 0;
}

.tags {
  margin-left: 10px;
}

.tag {
  background: #e0e0e0;
  padding: 2px 8px;
  border-radius: 3px;
  font-size: 0.85em;
  margin-right: 5px;
}

body.dark-mode .tag {
  background: #3d3d3d;
  color: #e0e0e0;
}

body.dark-mode .post-meta {
  color: #b0b0b0;
}

body.dark-mode .blog-post h2 a:hover {
  color: #6ab0f3;
}

.post-excerpt {
  margin: 15px 0;
  line-height: 1.6;
}

.read-more {
  color: #155799;
  text-decoration: none;
  font-weight: 500;
}

.read-more:hover {
  text-decoration: underline;
}

body.dark-mode .read-more {
  color: #6ab0f3;
}

.no-posts {
  text-align: center;
  padding: 40px 0;
  color: #666;
}

hr {
  border: none;
  border-top: 1px solid #eee;
  margin: 40px 0;
}

body.dark-mode hr {
  border-top-color: #444;
}
</style>
