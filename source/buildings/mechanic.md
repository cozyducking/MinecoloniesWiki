---
title: Minecolonies Wiki
layout: default
---
# Mechanic's Hut

<div class="infobox box text-center">
    <img src="../../assets/images/buildings/mechanic.png" alt="Mechanic" />
    <hr />
    <div class="row section-text text-left">
        <div class="col">
        <p><strong>Worker:</strong></p>
        </div>
        <div class="col">
        <p><a href="../workers/mechanic">Mechanic</a></p>
        </div>
    </div>
    <hr />
    <recipe>mechanic</recipe>
</div>

# About the Mechanic's Hut

The Mechanic's Hut is where the Mechanic will create redstone items, rail items, clocks, compasses, and other items not made by other crafters. For the Mechanic to work, they must receive a request from another worker and have the necessary materials. The Mechanic's Hut must also have been taught the crafting recipes for all the items you want the Mechanic to be able to craft.

**Hint:** The number of recipes you can teach the Mechanic's Hut doubles per building level. So:


| Mechanic's Hut Level | Number of Recipes |
| :-----: | :-----: |
| 1 | 20 | 
| 2 | 40 |
| 3 | 80 |
| 4 | 160 | 
| 5 | 320 | 

<br>

# Mechanic's Hut GUI

When accessing the Mechanic's Hut block by right-clicking on it, you will see a GUI with different options:

<div class="row">
  <div class="col-sm-12 col-md">
    <img src="../../assets/images/gui/mechanicgui.png" class="img-fluid mx-auto" alt="Mechanic GUI">
  </div>
  <div class="col-sm-12 col-md">
    <br>
    <ul>
      {% for item in site.data.gui.global %}
        <li><strong>{{ item.button }}:</strong> {{ item.content }}</li>
      {% endfor %}
    </ul>
  </div>
</div>
<br> <br>
