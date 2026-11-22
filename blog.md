---
layout: default
title: Notas & Finanzas
---
<div class="page-header">
  <h1>Notas de Finanzas, Riesgos & Regulación</h1>
  <p>Artículos breves que traducen conceptos técnicos de mercados financieros, economía y supervisión bancaria a análisis accesibles.</p>
</div>

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
  <div class="entry-card">
    <div class="entry-meta">{{ post.date | date: "%d %b %Y" }}</div>
    <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt | strip_html | truncatewords: 35 }}</p>
  </div>
  {% endfor %}
{% else %}
  <div class="entry-card">
    <div class="entry-meta">Próximamente</div>
    <h3>Serie: Fundamentos de Riesgo Financiero y Regulación Prudencial</h3>
    <p>Estoy preparando notas técnicas basadas en mis apuntes de finanzas cuantitativas, renta fija y supervisión financiera. Cada artículo creado en la carpeta <code>_posts/</code> aparecerá listado aquí automáticamente.</p>
  </div>
{% endif %}
