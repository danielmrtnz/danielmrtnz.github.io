<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography" style="margin-top: 0; margin-bottom: 0; padding-left: 0;">

{% for link in site.data.publications.main %}

<li style="margin-bottom: 5px; list-style: none; position: relative; padding-left: 15px;">
  <div style="position: absolute; left: 0; top: 0; padding-top: 2px;">•</div>
  <div style="padding-left: 5px;">
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
  </div>
</li>
{% endfor %}
</ol>
</div>
