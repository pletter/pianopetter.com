---
---
<nav id="newnav">
               <ul id="flexnav">
                   <a class="navbutton active" href="/"><li class="colorett leftborder"><span class="navbuttontext">Piano Blog</span></li></a>
                   <a class="navbutton " href="/pianotuition"><li class="colortva"><span class="navbuttontext whitetext">Piano Tuition</span></li></a>
                   <a class="navbutton" href="/pianoprojects"><li class="colorfem"><span class="navbuttontext">Piano Projects</span></li></a>
                   <a class="navbutton" href="/contactandpress"><li class="colorfyra"><span class="navbuttontext whitetext">Press and contact</span></li></a>
               </ul>
           </nav>

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
    