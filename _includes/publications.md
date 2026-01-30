<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
  <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
  <div class="author">{{ link.authors }}</div>
  <div class="periodical"><em>{{ link.journal }}</em></div>
  <div class="links">
    {% if link.pdf %} 
    <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
    {% endif %}
    <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
    {% if link.notes %} 
    <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
    {% endif %}
    {% if link.others %} 
    {{ link.others }}
    {% endif %}
  </div>
</li>
<br>

{% endfor %}

</ol>
</div>
