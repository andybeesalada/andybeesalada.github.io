---
layout: home
title: 3D Art & Animation Portfolio
---

Welcome to my graduate application portfolio. Below is a curated selection of my 3D assets, animations, and pipeline workflows developed in Blender.

---

## Featured Project: Character Turnaround & Topology

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin-bottom: 40px;">

  <!-- Left Column: Final Animation -->
  <div style="flex: 1; min-width: 320px;">
    <video autoplay loop muted playsinline width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
      <source src="{{ 'assets/videos/helical drift cancelling video.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <p style="text-align: center; font-size: 0.9em; color: #555; margin-top: 8px;"><b>Final Cycles Render</b><br>Lighting setup and surface textures.</p>
  </div>

  <!-- Right Column: Wireframe Breakdown -->
  <div style="flex: 1; min-width: 320px;">
    <img src="{{ '/assets/images/your-gif-name.gif' | relative_url }}" width="100%" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" alt="Topology Breakdown">
    <p style="text-align: center; font-size: 0.9em; color: #555; margin-top: 8px;"><b>Mesh Topology & Breakdown</b><br>Quad-dominant edge-loops optimized for deformation.</p>
  </div>

</div>

## Project Descriptions & Technical Notes
* **Software Used:** Blender, Substance Painter
* **Render Engine:** Cycles (1024 samples with OptiX Denoising)
* **Key Focus:** Clean hard-surface subdivision topology and photorealistic PBR texturing.
