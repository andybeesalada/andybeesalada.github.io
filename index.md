---
layout: home
title: "Charged Particle Motion in a Toroid: Tokamak"
---
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']]
    }
  };
</script>

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

Welcome to the portfolio I've made to organize my 3D animations made in Blender. I created these for my undergraduate senior thesis project, focusing on charged particle motion under electric and magnetic fields, specifically applied to the geometry of a tokamak nuclear fusion reactor. This presentation looked through the lens of single particle motion, though if I had more time I would have liked to explore further into magneto-hydrodynamics.<br>
Some physical realities are hard to visualize 100% true to life, so I took some creative liberties in these animations. My goal was to efficiently and accurately communicate these ideas during a limited presentation time, in the form of a slideshow. I felt that 3D animation would allow me to explain complicated concepts tied to the geometry of the nuclear reactors I researched.

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  How do charged particles behave under uniform magnetic fields?
</h2>


<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 320px;">
    <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/cyclo-gyration.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="text-align: center; font-size: 0.9em; color: #b0b0b0; margin-top: 8px;"><b>Cyclotron gyration</b><br>Charged particles gyrate under a uniform magnetic field, $\vec{B}$. No electric field here, so $\vec{E}=0$. The direction of gyration depends on the charge of the particle, $q$.</p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/cyclotron-helix-parts.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="With Nonzero Initial Velocity">
    <p style="text-align: center; font-size: 0.9em; color: #b0b0b0; margin-top: 8px;"><b>With $v_{\parallel}\neq0\;m/s$</b><br>Particles with nonzero initial velocity along the field line will keep that velocity, and gyrate around field lines.</p>
  </div>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  What if we vary the magnetic field or introduce an electric field?
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<!-- Central Focus Container -->
<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
  <img src="{{ 'assets/images/cyclotron-helix-parts-drift.png' | relative_url }}" width="100%" style="border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Cyclotron gyration with drift">
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Cyclotron gyration with added drift</b><br>
    Particles still gyrate around field lines, but now the center of their orbits drifts perpendicular to $\vec B$. This "guiding center drift" depends on changes in $\vec B$ and $\vec E$, because of the Lorentz force: $$ \vec F=q(\vec E+\vec v\times\vec B) $$
  </p>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  How do charged particles behave under spatially non-uniform magnetic fields?
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="max-width: 720px; margin: 0 auto 40px auto; font-size: 1.05em; line-height: 1.6; color: #e0e0e0; text-align: left;">
  
  The drift direction arising from a magnetic field gradient will point along the direction of $\vec B\times\vec{\nabla}B$. Oppositely charged particles will drift in opposite directions. The following animations display an upwards $\vec{\nabla}B$ direction (dark blue arrow), with $\vec B$ pointing out of the page (light blue).

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 400px;">
    <img src="{{ 'assets/images/speed-mag-grad-neg-drift.gif' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Negative particle gradient drift">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Negative particle drifting</b><br>
    A negative particle drifts to the right, opposite the result of $\vec B\times\vec{\nabla}B$.
  </p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 400px;">
    <img src="{{ 'assets/images/speed-mag-grad-pos-drift.gif' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Positive particle gradient drift">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Positive particle drifting</b><br>
    A positive particle drifts to the left, towards the result of $\vec B\times\vec{\nabla}B$.
  </p>
  </div>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  Setting up toroid axes
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="max-width: 720px; margin: 0 auto 40px auto; font-size: 1.05em; line-height: 1.6; color: #e0e0e0; text-align: left;">
  
  In order to get an understanding of what may cause a magnetic field gradient or an electric field in a tokamak fusion reactor, let's get a common understanding of axes and the geometry of a tokamak. For these examples, we'll use a simple ring torus example tokamak reactor.

</div>

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 400px;">
    <img src="{{ 'assets/images/toroidal-axes.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Tokamak toroidal axes">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Toroidal axes</b><br>
    We'll call the orange upward arrow $\hat z$. The pink arrow in-plane with the torus that is facing outwards is the "radial" axis, $\hat r$. Finally, the green ring     around the torus is the $\hat\theta$ axis, which we'll define to be counter-clockwise (towards the blue arrows). 
  </p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 400px;">
    <img src="{{ 'assets/images/poloidal-axis-pic.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Tokamak poloidal axes">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Poloidal axes</b><br>
    On this diagram, the axis of note is poloidal, the blue ring with orange arrows. We'll call this $\hat\phi$, and define to to be clockwise (towards the orange arrows). 
  </p>
  </div>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  Where does the toroidal magnetic field come from?
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
  <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/toroid-field-current-loops.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Poloidal current loops ($\vec I$) create toroidal $\vec B$</b><br>
    Imagine a solenoid, where tightly-wrapped current-carrying wire creates a straight magnetic field. Particles following these field lines will stream out of the end of the solenoid. But wrap it into a ring so the ends meet, and $\vec B$ becomes a circular path to trap particles.
  </p>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  Where do magnetic field gradients in a tokamak come from?
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
  <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/grad-explain-loops.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Cyclotron gyration with added drift</b><br>
    In a regular solenoid, $\vec B$ is spatially uniform and doesn't depend on position inside the solenoid's cross section. However, this is no longer true after wrapping it into a torus. Current loop density is higher on the inner radius of the torus than the outer radius, making $\vec B$ stronger when particles are closer to the torus "donut hole." This produces $\vec{\nabla}B$ that points towards $-\hat r$, radially inwards from weak field towards high.
  </p>

</div>
