---
permalink: /demo/
title: "Interactive demo"
excerpt: "Press a simulated GelSight-type tactile sensor in your browser and see the tactile image, the depth map recovered from it, and the marker displacement field."
author_profile: true
---

<p class="lead">A GelSight-type tactile sensor, simulated in your browser. Press the gel with the mouse or a finger, drag to shear it, and switch views to see what the camera records and what can be recovered from it.</p>

<iframe id="tactile-demo" class="demo-frame" src="/demos/tactile-sensor-demo.html" title="Interactive simulation of a GelSight-type tactile sensor"></iframe>

<p class="section-note">You can also <a href="/demos/tactile-sensor-demo.html">open the demo in its own window</a>. The real sensor I built is described in <a href="/portfolio/portfolio-1/">Building a GelSight-type tactile sensor</a>.</p>

## Physics-based simulator

<div class="demo-wrap">
  <a class="demo-card" href="/demos/gelsight-sim.html">
    <img src="/images/research/physics-sim-thumb.jpg" alt="Simulated camera image of a screw head pressed into a colour-only GelSight-type sensor">
    <span class="hl-body">
      <span class="hl-tag">Research tool · English / 中文</span>
      <span class="demo-title">A more physical simulator, with training-data export</span>
      <span class="hl-text">A colour-only sensor (no markers) in which each physical effect can be switched on and off and compared: elastic contact in a thin gel layer, coating reflectance and shadows, LED falloff and spectral crosstalk, light trapping and refraction in the gel, and camera noise. It exports images paired with height and normal maps, as training data for a network that replaces the lookup table.</span>
      <span class="demo-go">Open the simulator &rarr;</span>
    </span>
  </a>
</div>

<script>
  (function () {
    var frame = document.getElementById('tactile-demo');
    window.addEventListener('message', function (e) {
      if (e.source !== frame.contentWindow || !e.data || e.data.type !== 'tactile-demo:height') { return; }
      frame.style.height = e.data.height + 'px';
    });
  })();
</script>
