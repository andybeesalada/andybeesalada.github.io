---
layout: home
title: "Charged Particle Motion in a Toroid: Tokamak"
---
<style>
  /* Global Background & Text Colors */
  body {
    background-color: #121212 !important;
    color: #e0e0e0 !important;
  }

  /* Headings Color */
  h1, h2, h3, h4, h5, h6 {
    color: #ffffff !important;
    text-align: center !important;
  }

  /* Links Color */
  a {
    color: #64b5f6 !important;
  }

  /* Header / Title Bar Background & Accent */
  header, .site-header, .page-header {
    background-color: #2a2438 !important; /* Optional: dark muted purple container background */
    background-image: none !important;    /* Clears default theme blue gradients */
  }

  /* Site Title Font Color (Lilac / Pastel Purple) */
  .site-title, .page-title, .site-header a, header h1, header h2 {
    color: #c8b6ff !important;
  }

  /* Hover state for title link */
  .site-title:hover, .site-header a:hover {
    color: #e7c6ff !important;
  }
</style>

Welcome to my portfolio I've made to organize my 3D animations made in Blender. I created these for my undergraduate senior thesis project, focusing on charged particle motion under electric and magnetic fields, specifically applied to the geometry of a tokamak nuclear fusion reactor. Some physical realities are hard to visualize 100% true to life, so my goal was to make creative choices that helped me to explain these concepts in under 30 minutes of presentation time, using visuals in a PowerPoint.

---

## How do charged particles behave under uniform magnetic fields?


<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #333;">

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 320px;">
    <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/cyclo-gyration.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="text-align: center; font-size: 0.9em; color: #b0b0b0; margin-top: 8px;"><b>Cyclotron gyration</b><br>Charged particles gyrate under a uniform magnetic field (no electric field). The direction depends on the charge of the particle.</p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/cyclotron-helix-parts.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="With Nonzero Initial Velocity">
    <p style="text-align: center; font-size: 0.9em; color: #b0b0b0; margin-top: 8px;"><b>With nonzero initial velocity</b><br>Particles with nonzero initial velocity along the field line will keep that velocity, and gyrate around field lines.</p>
  </div>

</div>

## What if we vary the magnetic field, or introduce electric field?

---

<!-- Central Focus Container -->
<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
  <img src="{{ 'assets/images/cyclotron-helix-parts-drift.png' | relative_url }}" width="100%" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Cyclotron gyration with drift">
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b></b><br>
    .
  </p>

</div>


