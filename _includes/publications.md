<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<ol class="bibliography" style="padding-left: 0;">

{% for link in site.data.publications.main %}

<li style="margin-bottom: 1px;">
<div class="pub-row" style="padding-bottom: 5px;">
  <div class="col-sm-12" style="position: relative; padding-right: 15px; padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical" style="display: inline;"><em>{{ link.conference }}</em></div>
      <div class="links" style="display: inline;">
        {% if link.pdf %} 
        <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; margin-left: 10px;">PDF</a>
        {% endif %}
        {% if link.code %} 
        <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; margin-left: 5px;">Code</a>
        {% endif %}
        {% if link.page %} 
        <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; margin-left: 5px;">Project Page</a>
        {% endif %}
        {% if link.bibtex %} 
        <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; margin-left: 5px;">BibTex</a>
        {% endif %}
        {% if link.notes %} 
        <strong><i style="color:#e74d3c; margin-left: 5px;">{{ link.notes }}</i></strong>
        {% endif %}
        {% if link.others %} 
        <span style="margin-left: 5px;">{{ link.others }}</span>
        {% endif %}
      </div>
  </div>
</div>
</li>

{% endfor %}

</ol>
</div>
