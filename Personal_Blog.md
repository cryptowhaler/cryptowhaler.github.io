---
layout: page
title: "FIN-TECH to Finance SPACE-TECH"
subtitle: I write about :- <br> <br> 1. The potential impact of blockchain on established monetary & banking systems. <br> <br> 2. Digital Investment Assets that can support evolved Financially Engineered Products.  <br> <br> 3. Dapps that i am working upon. <br> <br> 4. How DLT based monetary systems can be created that can fuel space-tech research and space exploration. 
css: "/css/index.css"
meta-title: "Rahul Mittal - Fin-Tech Systems Architect"
meta-description: "Distributed Ledger based Financial Systems Architect and Developer, currently working with Societe Generale."
use-site-title: true
bigimg:
  - "/img/newCover.jpg" : "The Hero's Journey"

---


<div class="list-filters"> <!-- // USED TO IMPLEMENT FILTERS / SEGMENTATION ON POSTS -->
<a href="/index" class="list-filter">Latest</a> <!-- // No need to do anything for this -->
  <a href="/Finance" class="list-filter">Finance</a> <!-- // No need to do anything for this -->
  <a href="/DLT_Dapps" class="list-filter">De-Fi Dapps </a> <!-- // add a Explained Series.md file -->
  <a href="/Financial_Engineering" class="list-filter">Financial Engineering</a> <!-- add a Patent Analysis.md file -->
  <a href="/SpaceTech" class="list-filter">Space-Tech</a> <!-- // add a DLT_Dapps Aeronautical Analysis.md file  -->
  <a href="/Personal_Blog" class="list-filter  filter-selected">Personal Blogging</a> <!-- // add a DLT_Dapps Aeronautical Analysis.md file  -->

</div>


<div class="posts-list">
  {% for post in site.tags.Personal_Blog %}
  <article>
    <a class="post-preview" href="{{ post.url | relative_url  }}">
	    <h2 class="post-title">{{ post.title }}</h2>

	    {% if post.subtitle %}
	    <h3 class="post-subtitle">
	      {{ post.subtitle }}
	    </h3>
	    {% endif %}
      <p class="post-meta">
        Posted on {{ post.date | date: "%B %-d, %Y" }}
      </p>

      <div class="post-entry">
        {{ post.content | truncatewords: 50 | strip_html | xml_escape}}
        <span href="{{ post.url | relative_url  }}" class="post-read-more">[Read&nbsp;More]</span>
      </div>
    </a>  
   </article>
  {% endfor %}
</div>
