---
layout: default
---

{% include page-intro.html %}

<main id="main" class="page-content" aria-label="Content">
  <div class="index inner">
    <div>
      <header class="section-title">
        <h2>Documents</h2>
      </header>
      <div class="entries">
          {% assign files = site.static_files | where: "class", page.classe %}
          <ul>
          {% for f in files %}
            <li><a href="{{ f.path }}">{{ f.name }}</a></li>
          {% endfor %}
          </ul>
      </div>
      
    </div>

    {% include footer.html %}
  </div>
</main>
