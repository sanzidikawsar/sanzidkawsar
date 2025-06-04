---
permalink: /
title: "About Sanzid"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I am a self-taught AI engineer & datascience researcher..

Currently, a PhD candidate and researcher at King Abdulaziz University, specializing in Data Science with a focus on Machine Learning, Natural Language Processing (NLP), and Generative AI. Prior to my doctoral studies, I served as a University Faculty at Daffodil International University, where I was actively involved in teaching and research. My work bridges theoretical foundations and real-world applications, with ongoing projects exploring advanced models in AI and data-driven solutions to complex problems.

Let me know if you'd like to highlight specific projects, publications, or research interests.


<h2>Recent Posts</h2>
<div class="recent-posts-blocks" style="display: flex; flex-wrap: wrap; gap: 1.2rem; margin-bottom: 1.2rem;">
  {% for post in site.posts limit:5 %}
    <div class="post-block" style="background: #f8f9fa; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.05); padding: 0.7rem 0.8rem; min-width: 220px; max-width: 320px; flex: 1 1 220px;">
      <a href="{{ post.url | relative_url }}" style="font-size: 1.05rem; font-weight: bold; color: #2a2a2a; text-decoration: none;">
        {{ post.title }}
      </a>
      <div style="font-size: 0.88rem; color: #888; margin: 0.2rem 0 0.5rem 0;">
        {{ post.date | date: "%B %d, %Y" }}
      </div>
      {% if post.excerpt %}
        <div class="post-short-desc" style="font-size: 0.95rem; color: #444;">
          {{ post.excerpt | strip_html | truncate: 120 }}
        </div>
      {% endif %}
    </div>
  {% endfor %}
</div>


