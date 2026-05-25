<h2 id="publications" class="publications-heading">Publications <span class="publication-footnote">(* denotes equal contribution)</span></h2>

<div class="publications">
<ol class="bibliography publication-list">

{% for link in site.data.publications.main %}

<li>
<article class="pub-row">
  <div class="pub-media">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser" alt="{{ link.title }} teaser">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  <div class="pub-body">
    <div class="title">
      {% if link.pdf %}
      <a href="{{ link.pdf }}" target="_blank" rel="noopener">{{ link.title }}</a>
      {% else %}
      {{ link.title }}
      {% endif %}
    </div>
    <div class="author">{{ link.authors }}</div>
    <div class="periodical"><em>{{ link.conference }}</em></div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" rel="noopener">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <span class="pub-note">{{ link.notes }}</span>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</article>
</li>

{% endfor %}

</ol>
</div>
