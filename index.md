---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
permalink: /
---

{% include header.html %}

<main class="page-content" aria-label="Content">
  <div class="wrapper">
    <div class="home">
      <h1>Hi! I'm Anith.</h1>
      <p> //Description. </p>
      
      <h2 class="post-list-heading">Work</h2>
      {% for post in site.posts %}
      <ul class="post-list">
        <li>
          <span class="post-meta">Jun 18, 2018</span>
          <h3><a class="post-link" href=" {{post.link}} ">{{ post.title }}</a></h3>
          <span style="font-size: 16px;">Swinburne University timetable application redesign.</span>
          {{ post.excerpt }}
        </li>
        <li><span class="post-meta">Feb 1, 2018</span>
        <h3>
          <a class="post-link" href="/case-studies/2018/02/01/nattlampa.html">
            Nattlampa
          </a>
          <span style="font-size: 16px;">App that measures the impact of artificial night-time lighting on nocturnal wildlife.</span>
        </h3></li></ul>

      </div>
    </main>
    
{% include footer.html %}
