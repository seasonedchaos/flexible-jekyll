---
name: Kurt Hansen
layout: main
---

<article class="article-page">
  <div class="page-content">
    <h2>Kurt Hansen</h2>
    <p><img src="{{ site.url }}/assets/img/Hansen_headshot.jpg" alt="Kurt Hansen headshot" width="40%" align="left" hspace="30">I am a postdoc at the Naval Research Lab in Monterey, CA. I got my Ph.D. in atmospheric science from the University of Miami RSMAS under Sharan Majumdar and Ben Kirtman. My research focuses on subseasonal variability of Atlantic and Pacific tropical cyclone activity. I received my Bachelors in atmospheric science at the University of Albany. In my free time I like rock climbing, card games, and long romantic unicycle rides by the beach. </p>
    <a href="https://twitter.com/all4hurricanes1" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i></a><br><br><br><br><br><br><br><br><br><br><br><br>
    <h2>Posts by {{ page.name }}:</h2>
    <ul>
    {% for post in site.posts %}
      {% assign authorCount = page.authors | size %}
      {% for author in post.authors %}
        {% if author == page.name %}
          <div class="tag-list">
            <span><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></span>
            <small><span>| {{ post.date | date_to_string }}</span></small>
          </div>
        {% endif %}
      {% endfor %}
    {% endfor %}
    </ul>
  </div> <!-- End Page Content -->
</article> <!-- End Article Page -->
