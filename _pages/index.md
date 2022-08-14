---
layout: page
title: Home
id: home
permalink: /
---

<h1 class="title">Chris Martin</h1>

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
    {% assign sorted = site.notes | sort: 'date' | reverse %}
    {% for item in sorted %}
      <li>
        <a href="{{ item.url }}">{{ item.title }}</a>
        <br>
        <small class="date">{{ item.date | date: '%B %d, %Y' }}</small>
      </li>
    {% endfor %}
  </ul>
</div>

<style>
  .wrapper {
    max-width: 46em;
  }
  li { padding: 0.5em; margin: 0.7em; }
  nav { display: none; }
</style>
