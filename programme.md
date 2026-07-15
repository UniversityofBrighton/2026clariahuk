---
layout: default
title: Programme
subtitle: A single day of talks, panels and lightning sessions on the infrastructures behind research. The full schedule will be published here — this is the shape it will take.
---

<main>
  <div class="wrap">
    <div class="section-head">
      <h2>Provisional schedule</h2>
      <span class="tag">TO BE CONFIRMED</span>
    </div>

    <div class="schedule">
      {% for slot in site.data.schedule %}
      <div class="slot">
        <div class="time">{{ slot.time }}</div>
        <div>
          <div class="title">{{ slot.title }}</div>
          <div class="desc">{{ slot.note }}</div>
        </div>
      </div>
      {% endfor %}
    </div>

    <p class="note">Edit sessions in <code>_data/schedule.yml</code>.</p>
  </div>
</main>
