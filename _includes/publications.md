<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography" style="margin-top: 0; margin-bottom: 0; list-style-type: decimal; padding-left: 25px;">

{% for link in site.data.publications.main %}

<li style="margin-bottom: 1px; display: list-item;">
  <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
  <div class="author">{{ link.authors }}</div>
  <div class="details">
    <em>{{ link.journal }}</em>
    {% if link.notes %}
    <strong style="color:#e74d3c; margin-left: 10px;">{{ link.notes }}</strong>
    {% endif %}
    <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; margin-left: 10px;">BibTex</a>
    {% if link.others %}
    <span style="margin-left: 10px;">{{ link.others }}</span>
    {% endif %}
  </div>
</li>

{% endfor %}
</ol>
</div>
