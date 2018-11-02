---
---
<nav id="newnav">
               <ul id="flexnav">
                   <a class="navbutton active" href="https://pletter.github.io/pianopetter.com/"><li class="colorett"><span class="navbuttontext">Blog</span></li></a>
                   <a class="navbutton" href="https://pletter.github.io/pianopetter.com/teaching"><li class="colortva"><span class="navbuttontext">Teaching</span></li></a>
                   <a class="navbutton" href="https://pletter.github.io/pianopetter.com/previouswork"><li class="colorfem"><span class="navbuttontext">Projects</span></li></a>
                   <a class="navbutton" href="https://pletter.github.io/pianopetter.com/contactandpress"><li class="colorfyra"><span class="navbuttontext">Press and contact</span></li></a>
               </ul>
           </nav>

{% for post in site.posts %}
<article class="episode">
    <h1>
        
            {{ post.title }}
    </h1>

    <div class="shownotes">
        {{ post.content }}
    </div>
    <p class="meta">
        <time datetime="{{ post.date | date: "%Y-%m-%d" }}">
            {{ post.date | date: "%Y-%m-%d" }}
        </time>
    </p>
</article>
{% endfor %}
    