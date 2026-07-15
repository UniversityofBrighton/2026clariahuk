---
layout: default
title: About the event
subtitle: Bringing together researchers, academics, and museum & library professionals to shape the digital and physical infrastructures that underpin research.
---

<main>
  <div class="wrap">
    <div style="max-width:720px;margin-bottom:56px">
      <h2 style="font-size:30px;margin-bottom:16px">Why we're meeting</h2>
      <p class="lead">Edit this section in <code>about.md</code>. A short introduction to the event's purpose: the shared systems, data, tools and partnerships that research depends on, and why the community is gathering in Brighton to strengthen them.</p>
    </div>

    <h2 style="font-size:26px;margin-bottom:22px">Themes</h2>
    <div class="themes">
      {% for t in site.data.about.themes %}
      <div class="theme">
        <div class="num">{{ t.num }}</div>
        <div class="title">{{ t.title }}</div>
        <div class="text">{{ t.text }}</div>
      </div>
      {% endfor %}
    </div>

    <h2 style="font-size:26px;margin-bottom:18px">Who it's for</h2>
    <div class="chips">
      {% for a in site.data.about.audiences %}
      <span class="chip">{{ a }}</span>
      {% endfor %}
    </div>

    <div class="org-grid">
      <div>
        <div class="k-label">ORGANISED BY</div>
        <div class="serif" style="font-size:20px;line-height:1.5">{% for host in site.hosts %}{{ host }}{% unless forloop.last %}<br />{% endunless %}{% endfor %}</div>
      </div>
      <div>
        <div class="k-label">PARTNERS &amp; SUPPORTERS</div>
        <div class="logos">
          <div class="logo-slot">LOGO</div>
          <div class="logo-slot">LOGO</div>
          <div class="logo-slot">LOGO</div>
        </div>
      </div>
    </div>
  </div>
</main>
