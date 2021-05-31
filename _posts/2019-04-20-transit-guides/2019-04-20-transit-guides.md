---
title: Transit Guides
tags: work dev design transit
accent: purple
tile:
  order: 3
  width: 5
  height: 7
  image: tile.svg
feature:
  width: 17
  height: 9
  image: feature.svg
image: https://cdn.glitch.com/d3e253ff-871d-442c-988d-a70ce0de1dc3/transit-guides-meta-preview.png?v=1604549022913
---

I created a series of mobile-friendly and printable web-based guides to help college students find their way around the Philadelphia area on public transit. 🚈🚌🚎🚋

> Links to guides for participating schools: <a href="https://septayac.com/haverford" target="_blank" rel="noreferrer">Haverford College</a> ♦ <a href="https://septayac.com/brynmawr" target="_blank" rel="noreferrer">Bryn Mawr College</a> ♦ <a href="https://septayac.com/immaculata" target="_blank" rel="noreferrer">Immaculata University</a> ♦ <a href="https://septayac.com/harcum" target="_blank" rel="noreferrer">Harcum College</a> ♦ <a href="https://septayac.com/sju" target="_blank" rel="noreferrer">St. Joseph's University</a> ♦ <a href="https://septayac.com/swarthmore/" target="_blank" rel="noreferrer">Swarthmore College</a> ♦ <a href="https://septayac.com/delval" target="_blank" rel="noreferrer">Delaware Valley University</a> ♦ <a href="https://septayac.com/usciences/" target="_blank" rel="noreferrer">USciences</a> ♦ <a href="https://septayac.com/upenn" target="_blank" rel="noreferrer">UPenn</a>

---

As part of my advisory role with SEPTA (Southeastern Pennsylvania Transportation Authority), I collaborated with the members of the Youth Advisory Council to update new rider resources distributed to schools in the area. The existing resources consisted of brochures that needed to be individually updated in Microsoft Publisher, and often contained outdated information.

Consulting with students new to the area and/or have never ridden public transit before in small focus groups, I turned these brochures into web-based guides that are digital-first. It put forward resources pertaining to the 3 most commonly asked questions by students:

- Where are the stops?
- How much does it cost? How to I pay?
- What does the train/bus take me?

[Web guide for Bryn Mawr College: ![webpage](https://cdn.glitch.com/2d246102-8341-4166-a220-b39d607c9218/transit-guides-header.png?1555779821247)](https://pixelyunicorn.github.io/septa-guides/brynmawr/)

At the bottom of each guide, there is a card layout that allows information to be kept up to date between guides. (This is especially important for fare changes or the rollout of new payment methods.)

![card](https://cdn.glitch.com/2d246102-8341-4166-a220-b39d607c9218/transit-guides-card.png?1555789809691)

You can even print these pages to generate brochures using your browser's built-in print command. Printed brochures are distributed at information desks and new student orientations at colleges throughout the Philadelphia area.

[Printed guide for Bryn Mawr College: ![print preview](https://cdn.glitch.com/2d246102-8341-4166-a220-b39d607c9218/transit-guides-print-preview.png?1555779821247)](https://pixelyunicorn.github.io/septa-guides/pdf/septa-yac-bryn-mawr-college.pdf)

A [simple YAML file](https://github.com/pixelyunicorn/septa-guides/blob/master/pages/immaculata.md) provides the data for each of the guides. Information such as fares, maps, and walking directions are automatically generated (and kept up to date) based on what is provided in the YAML file. 

<blockquote markdown="block">
  
```yaml
---
layout: guide
title: Immaculata University
cover: /images/cover-immaculata.jpg
permalink: /immaculata/
zone: 4
lat: 40.0273391
lon: -75.5707867
methods:
- mode: bus
  name: Route 92
  frequency: Every 30-90 minutes
  route: Exton to King of Prussia
  station: Stops throughout West King Rd
  address: King Rd & Immaculata Dr, Immaculata, PA
  lat: 40.026764
  lon: -75.571116
  destinations:
  - To Exton - Exton Square Mall ...
  - To King of Prussia - Malvern Regional Rail ...
- mode: rr
  name: Paoli-Thorndale Line
  frequency: Every 15-30 minutes
  route: Thorndale to Center City Philadelphia
  station: Malvern Regional Rail Station
  zone: 4
  address: 54 N Bryn Mawr Ave, Bryn Mawr, PA 19010
  lat: 40.0366623
  lon: -75.5176516
  destinations:
    - Sports and Entertainment Complexes
    - Train/Bus to New York City
    - Train to Philadelphia International Airport
    - Shopping Destinations
    - Museums, Art, and Cultural Venues
---
```

</blockquote>

Since rolling out these new guides, over 2500+ students have utilized them to find essential information on stops, routes, and fares relevant to their schools!

![person picking up a magnet from a table](https://cdn.glitch.com/2d246102-8341-4166-a220-b39d607c9218/transit-guides-table.jpg?1555790350650)

_(Links to these guides can be found at the top of this post.)_