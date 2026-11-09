---
permalink: /demo/
title: "Interactive demo"
excerpt: "Press a simulated GelSight-type tactile sensor in your browser: a basic version with depth and marker views, and a physics-based version of the colour-only sensor."
author_profile: true
---

<p class="lead">A GelSight-type tactile sensor, simulated in your browser. Press the gel with the mouse or a finger and drag to shear it. <b>Basic</b> shows what the camera records and what can be recovered from it; <b>Physics-based</b> models the gel, the light and the camera in more detail.</p>

<div class="demo-tabs" role="tablist" aria-label="Demo version">
  <button type="button" class="demo-tab" role="tab" id="tab-basic" aria-selected="true" aria-controls="tactile-demo" data-frame="tactile-demo">Basic</button>
  <button type="button" class="demo-tab" role="tab" id="tab-physics" aria-selected="false" aria-controls="physics-demo" data-frame="physics-demo" data-hash="physics">Physics-based</button>
</div>

<iframe id="tactile-demo" class="demo-frame" role="tabpanel" aria-labelledby="tab-basic" src="/demos/tactile-sensor-demo.html" title="Interactive simulation of a GelSight-type tactile sensor"></iframe>

<iframe id="physics-demo" class="demo-frame" role="tabpanel" aria-labelledby="tab-physics" data-src="/demos/gelsight-sim.html" title="Physics-based simulation of a colour-only GelSight-type tactile sensor" hidden="hidden"></iframe>

<p class="section-note">Open in its own window: <a href="/demos/tactile-sensor-demo.html">basic</a> &middot; <a href="/demos/gelsight-sim.html">physics-based</a>. The real sensor I built is described in <a href="/portfolio/portfolio-1/">Building a GelSight-type tactile sensor</a>.</p>

<script>
  (function () {
    var tabs = document.querySelectorAll('.demo-tab');
    var frames = { 'tactile-demo': 'tactile-demo:height', 'physics-demo': 'gelsight-sim:height' };
    function show(tab) {
      for (var i = 0; i < tabs.length; i++) {
        var t = tabs[i], f = document.getElementById(t.getAttribute('data-frame')), on = t === tab;
        t.setAttribute('aria-selected', on ? 'true' : 'false');
        t.tabIndex = on ? 0 : -1;
        f.hidden = !on;
        if (on) {
          if (!f.getAttribute('src')) { f.setAttribute('src', f.getAttribute('data-src')); }
        }
      }
    }
    for (var i = 0; i < tabs.length; i++) {
      tabs[i].addEventListener('click', function () {
        show(this);
        var h = this.getAttribute('data-hash');
        if (window.history.replaceState) { window.history.replaceState(null, '', h ? '#' + h : location.pathname + location.search); }
      });
      tabs[i].addEventListener('keydown', function (e) {
        if (e.key !== 'ArrowLeft') { if (e.key !== 'ArrowRight') { return; } }
        var n = this === tabs[0] ? tabs[1] : tabs[0];
        n.focus(); n.click(); e.preventDefault();
      });
    }
    if (location.hash === '#physics') { show(tabs[1]); }
    window.addEventListener('message', function (e) {
      if (!e.data) { return; }
      for (var id in frames) {
        var f = document.getElementById(id);
        if (e.source === f.contentWindow) {
          if (e.data.type === frames[id]) { if (e.data.height > 50) { f.style.height = e.data.height + 'px'; } }
        }
      }
    });
  })();
</script>
