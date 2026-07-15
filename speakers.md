---
layout: default
title: Speakers
subtitle: Researchers, practitioners and policy voices from across the UK and Europe. Confirmed speakers will appear here as the line-up takes shape.
---

<main>
  <div class="wrap">
    <div class="section-head">
      <h2>Confirmed line-up</h2>
      <span class="tag">TO BE ANNOUNCED</span>
    </div>

    <div class="speakers">
      {% for sp in site.data.speakers %}
      <div class="speaker">
        <div class="photo">
          {% if sp.photo %}
          <img src="{{ sp.photo | relative_url }}" alt="{{ sp.name }}" />
          {% else %}
          <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#b6ad9b" stroke-width="1.5"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4 3.5-6 8-6s8 2 8 6"/></svg>
          {% endif %}
        </div>
        <div class="name">{{ sp.name }}</div>
        <div class="role">{{ sp.role }}</div>
      </div>
      {% endfor %}
    </div>

    <p class="note">Edit speakers in <code>_data/speakers.yml</code>.</p>
  </div>
</main>
