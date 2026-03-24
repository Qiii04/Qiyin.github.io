<h2 id="projects" style="margin: 2px 0px -15px;">Projects</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.projects.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="padding-right: 15px;">
    {% if link.image %}
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1">
    {% endif %}
  </div>

  <div class="col-sm-9" style="padding-left: 20px;">
      <div class="title">
        {% if link.link %}
        <a href="{{ link.link }}">{{ link.title }}</a>
        {% else %}
        {{ link.title }}
        {% endif %}
      </div>

      <div class="author">{{ link.authors }}</div>

      <div class="periodical">
        {{ link.description }}
      </div>

  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>
