---
---


{% for post in site.posts %}
<article class="blogpost">
   
    <div class="blogtext">
        <h2>
                {{ post.title }}
        </h2>
        
        {{ post.content }}
    </div>
    <p class="meta">
        <time datetime="{{ post.date | date: "%Y-%m-%d" }}">
            {{ post.date | date: "%Y-%m-%d" }}
        </time>
    </p>
</article>
{% endfor %}
    