---
layout: default
title: Venue & travel
subtitle: The event is held at the University of Brighton, a short walk from the seafront and the Royal Pavilion. Full directions and access information will be published here.
---

<main>
  <div class="wrap">
    <div class="venue-grid">
      <div>
        <div class="map">
          <svg width="44" height="44" viewBox="0 0 24 24" fill="none" stroke="#b6ad9b" stroke-width="1.5"><path d="M12 21s-6-5.3-6-10a6 6 0 0 1 12 0c0 4.7-6 10-6 10Z"/><circle cx="12" cy="11" r="2.2"/></svg>
          <span>MAP / VENUE PHOTO</span>
        </div>
        <div style="margin-top:20px">
          <div class="serif" style="font-size:22px">University of Brighton</div>
          <div style="font-size:15px;color:var(--muted);margin-top:4px">Grand Parade, Brighton, BN2 0JY · placeholder address</div>
        </div>
      </div>
      <div class="travel">
        {% for b in site.data.travel %}
        <div class="block">
          <div class="k">{{ b.label }}</div>
          <div class="t">{{ b.text }}</div>
        </div>
        {% endfor %}
      </div>
    </div>
    <p class="note">Edit directions in <code>_data/travel.yml</code>; the intro text is in <code>venue.md</code>.</p>
  </div>
</main>
