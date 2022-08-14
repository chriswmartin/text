---
layout: page
title: Home
id: home
permalink: /
---

<div class="box" id="who-am-i">
<h2>Contact me: </h2>
  <ul>
    <li>Email: <a href="mailto:me@chriswm.com">me@chriswm.com</a></li>
  </ul>
</div>

<div class="box" id="writing">
  <h2>Projects & writing:</h2>
  <ul>
  <!-- <ul style="padding: 3em; background: #f5f7ff; border-radius: 4px;"> -->
    {% for post in site.notes %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <br>
        <small class="date">{{ post.date | date: '%B %d, %Y' }}</small>
      </li>
    {% endfor %}
  </ul>
</div>

<style>
  .wrapper {
    max-width: 46em;
  }
  li { padding: 0.5em; margin: 0.7em; }
</style>
