---
title: Muziek pagina
date: 2021-06-11 12:04:00 Z
layout: page
---

> Muziek geeft je kriebels

lorem20
  <ul>
        {% for post in site.samenspel %}
        <li>
           <div class="nieuws__title-wrap">
               <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
                <p>{{ post.date | date_to_string }}</p>
           </div>
            <p>{{ post.excerpt | truncate: 55 }}</p>
            <p>{{ post.map.instrumenten }}</p>
            <p style="color:red; font-weight:bold;">{{ map.instrumenten }}</p>
        </li>
        {% endfor %}
    </ul>
