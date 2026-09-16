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
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/toroid-axes-labelled.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Tokamak toroidal axes">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Toroidal axes</b><br>
    We'll call the orange upward arrow $\hat z$. The pink arrow in-plane with the torus that is facing outwards is the "radial" axis, $\hat r$. Finally, the green ring     around the torus is the $\hat\theta$ axis, which we'll define to be counter-clockwise (towards the blue arrows). 
  </p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/poloidal-axis-labelled.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Tokamak poloidal axes">

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
    <b>Poloidal current loops ($\vec I$, light yellow lines) create toroidal $\vec B$</b><br> (light blue lines)
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
    In a regular solenoid, $\vec B$ is spatially uniform and doesn't depend on position inside the solenoid's cross section. However, this is no longer true after wrapping it into a torus. Current loop density is higher on the inner radius of the torus than the outer radius, making $\vec B$ stronger when particles are closer to the torus "donut hole." This produces $\vec{\nabla}B$ that points towards $-\hat r$, radially inwards from weak field towards high.<br>
    The inner blue line segment represents the gap between inner radius current loops, and the orange represents outer radius ones. The difference is more pronounced and noticeable if you shrink the inner radius compared to outer.
  </p>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  What drifts come from this magnetic field gradient?
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/grad-drift-gradient-inward.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Tokamak toroidal axes">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Toroid axes with gradient vector</b><br>
    This diagram shows the axes of our torus with the $\vec{\nabla}B\rightarrow -\hat r$ vector in dark blue. The magnetic field $\vec B$ is in light blue, along $\hat\theta$.
  </p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/grad-drift-directions-basic.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Tokamak poloidal axes">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Positive and negative particle drift directions</b><br>
    The cross product $\vec B\times\vec{\nabla}B$ points towards $\hat z$. Positive particles will then drift towards $+\hat z$, while negative will drift towards $-\hat z$. This results in charge separation, and an electric field pointing from positive particles to negative, or towards $-\hat z$.
  </p>
  </div>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  Now that we have an electric field as well, what happens?
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/e-cross-b-parts-drift.gif' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="E cross B perpendicular drift gif">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>$\vec E\times\vec B$ drift</b><br>
    This GIF shows the drift directions of positive particles, where $\vec E$ points downward and $\vec B$ points out of the page. Both positive and negative particles drift the same direction.
  </p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/grad-drift-directions-basic.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="E cross B perpendicular drift no init v gif">

  <!-- Caption -->
  <p style="font-size: 0.95em; text-align: center; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>temp</b><br>
    temp.
  </p>
  </div>

</div>

<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
 <img src="{{ 'assets/images/ecross-drift-basic.png' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="E cross B Drift Directions">
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Drift due to electric field from gradient charge separation</b><br>
    We now know that there will be an electric field, pointing towards $-\hat z$, due to the charge separation caused by gradient drifts. The drift caused by this electric field will point towards the cross product $\vec E\times\vec B$, but will not depend on the particle's charge, $q$. Both negative and positive particles will drift in the same direction.<br> Anywhere on the torus, the result of $\vec E$ crossed with $\vec B$ will point radially outwards, towards $\hat r$. So, positive and negative particles alike get flung outwards against the walls of our reactor.
  </p>

</div>

<h2 style="text-align: center; margin-top: 35px; margin-bottom: 10px;">
  Putting the drifts together
</h2>

<hr style="margin-top: 10px; margin-bottom: 30px; border: 0; border-top: 1px solid #ffffff;">

<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
 <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/toroidal-drifts-parts.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Combined drifts in tokamak (particles)</b><br>
    From the $\vec \nabla B$ drift we know positive particles drift up, negative drift down. From the $\vec E\times\vec B$ drift we know all particles drift radially outwards. Put together, positive drifts up and out, negative drifts down and out. Fusion reactions occur more frequently at higher temperatures, but the particles in our reactor will collide with walls and transfer energy away. Not ideal for a sustained reaction.
  </p>

</div>

<div style="max-width: 720px; margin: 0 auto 40px auto; text-align: center;">

  <!-- Main Video / Image -->
 <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/toroidal-drifts-rings.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  
  <!-- Caption & Description -->
  <p style="font-size: 0.95em; color: #b0b0b0; margin-top: 12px; line-height: 1.5;">
    <b>Combined drifts in tokamak (ring orbit representation)</b><br>
    The charged particles will always have their cyclotron gyration around the magnetic field lines, which we can see from the Lorentz force. However, these orbits don't cause problems like heat transfer to walls, because on average, cyclotron gyration will keep the particles in the same general area. So, it can be useful when doing calculations like these to average motion over full cyclotron gyrations. This leaves us with the more important components of motion, like $\vec\nabla B$ and $\vec E\times\vec B$ drifts. <br>That is why I made two versions of this animation, one with the particles represented as orbs/points, and another with just the orbit represented as a ring. This makes it easier to follow the motion of the guiding center, and see that the drift is vertical and radially outwards.
  </p>

</div>

