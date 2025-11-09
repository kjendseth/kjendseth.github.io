---
layout: page
permalink: /blog/
title: daily life
nav: true
nav_order: 1
galleries:
  - title: Lab life at NMBU
    description: Snapshots from daily research—robots, spectroscopy rigs, and the campus that hosts them.
    images:
      - assets/img/gallery/nmbu/campus.jpeg
      - assets/img/gallery/nmbu/epr_lab.jpeg
      - assets/img/gallery/nmbu/voltammetry.jpeg
      - assets/img/gallery/nmbu/3d_printing.jpeg
      - assets/img/gallery/nmbu/ot_2_robot_protein_crystallization.jpeg
      - assets/img/gallery/nmbu/homebuilt_robot.jpeg
      - assets/img/gallery/nmbu/homebuilt_robot_working.jpeg
      - assets/img/gallery/nmbu/building_robot.jpeg
      - assets/img/gallery/nmbu/robot.jpeg
      - assets/img/gallery/nmbu/eika.jpeg
      - assets/img/gallery/nmbu/outdoors.jpeg
  - title: Beamtime & Grenoble trips
    description: ESRF nights, Alpine mornings, and every group selfie we remembered to take.
    images:
      - assets/img/gallery/grenoble/esrf_robot.jpeg
      - assets/img/gallery/grenoble/group_work_esrf.jpeg
      - assets/img/gallery/grenoble/lab_esrf.jpeg
      - assets/img/gallery/grenoble/lab_2_esrf.jpeg
      - assets/img/gallery/grenoble/lab_3_esrf.jpeg
      - assets/img/gallery/grenoble/laser_esrf.jpeg
      - assets/img/gallery/grenoble/group_esrf_1.jpeg
      - assets/img/gallery/grenoble/group_grenoble.jpeg
      - assets/img/gallery/grenoble/group_alps_grenoble.jpeg
      - assets/img/gallery/grenoble/group_alps.jpeg
      - assets/img/gallery/grenoble/alps_grenoble.jpeg
      - assets/img/gallery/grenoble/me_group_grenoble.jpeg
      - assets/img/gallery/grenoble/group_collegaus_grenoble.jpeg
      - assets/img/gallery/grenoble/group_annecy.jpeg
      - assets/img/gallery/grenoble/food_grenoble.jpeg
      - assets/img/gallery/grenoble/cheese_grenoble.JPG
      - assets/img/gallery/grenoble/dessert_grenoble.jpeg
      - assets/img/gallery/grenoble/esrf_outdoors.jpeg
---

{% for gallery in page.galleries %}

<section class="mb-5">
  <h2>{{ gallery.title }}</h2>
  <p>{{ gallery.description }}</p>
  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
    {% for image in gallery.images %}
    <div class="col">
      <div class="card border-0 shadow-sm h-100">
        <img src="{{ image | relative_url }}" class="card-img-top" alt="{{ gallery.title }} photo">
      </div>
    </div>
    {% endfor %}
  </div>
</section>
{% endfor %}
