---
layout: home
title: Charged Particle Motion in a Toroid Tokamak
---

Welcome to my portfolio I've made to organize my 3D animations made in Blender. I created these for my undergraduate senior thesis project, focusing on charged particle motion under electric and magnetic fields, specifically applied to the geometry of a tokamak nuclear fusion reactor. Some physical realities are hard to visualize 100% true to life, so my goal was to make creative choices that helped me to explain these concepts in under 30 minutes of presentation time, using visuals in a PowerPoint.

---

## Featured Project: Character Turnaround & Topology

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 320px;">
    <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/helical-drift-cancel.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="text-align: center; font-size: 0.9em; color: #555; margin-top: 8px;"><b>Final Cycles Render</b><br>Lighting setup and surface textures.</p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ 'assets/images/speed-mag-grad-neg-drift.gif' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Topology Breakdown">
    <p style="text-align: center; font-size: 0.9em; color: #555; margin-top: 8px;"><b>Mesh Topology & Breakdown</b><br>Quad-dominant edge-loops optimized for deformation.</p>
  </div>

</div>

## Project Descriptions & Technical Notes
* **Software Used:** Blender, Substance Painter
* **Render Engine:** Cycles (1024 samples with OptiX Denoising)
* **Key Focus:** Clean hard-surface subdivision topology and photorealistic PBR texturing.
