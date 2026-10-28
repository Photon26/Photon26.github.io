---
title: "Rotational scanning for a wider field of view"
collection: portfolio
order: 1
period: "2026"
venue: "IEEE Sensors Journal"
thumb: rotating-thumb.jpg
thumb_alt: "Rotational-scanning tactile sensor beside a ruler"
result: "Field-of-view width 10 → 28 mm, without making the sensor thicker."
paper: "https://doi.org/10.1109/JSEN.2026.3668906"
excerpt: "A thin pinhole tactile sensor whose imaging module rotates to scan the contact surface, widening the effective field of view from 10 mm to 28 mm."
---

<figure class="fig">
  <img src="/images/research/rotating-overview.jpg" alt="Rotational-scanning tactile sensor beside a ruler, with a raw RGB image and the reconstructed depth map">
  <figcaption>The sensor beside a ruler, with a raw RGB image and the reconstructed depth map.</figcaption>
</figure>

**Problem.** A pinhole camera placed close to the elastomer keeps a tactile sensor thin, but it sees only a small patch of the contact surface. My previous static pinhole prototype covered a width of 10 mm.

**Approach.** I designed a thin geared mechanism that rotates the pinhole module, driven by a Dynamixel motor mounted behind the fingertip. The rotation center is estimated from tracked markers with least squares and RANSAC, and the registered frames are blended with center weighting into a single 28 × 28 mm depth map.

<figure class="fig">
  <img src="/images/research/rotating-design.jpg" alt="Exploded CAD view of the motor, transmission gears and finger module">
  <figcaption>Motor, transmission and finger modules. The gear connector rotates the pinhole sheet and camera above the light guide and elastomer.</figcaption>
</figure>

**Result.** The effective field-of-view width grew from 10 mm to 28 mm, and the sensing part ended up slightly thinner than the static prototype (15.0 → 14.3 mm). The evaluation also traced a systematic depth underestimation at object boundaries to the object blocking light inside the light guide.

<figure class="fig">
  <img src="/images/research/rotating-objects.jpg" alt="Seven test objects with their RGB images and reconstructed depth images">
  <figcaption>Seven test objects, their RGB images, and the reconstructed depth.</figcaption>
</figure>

**My role.** Lead researcher and first author: mechanism and optical design, prototyping, calibration, reconstruction, evaluation and writing.

**Paper.** Y. Gao, S. Zhang, W. Wan, B. Fang, F. Sun and K. Harada, "A Thin Pinhole-Based Tactile Sensor With Rotational Scanning for Field-of-View Expansion," *IEEE Sensors Journal*, vol. 26, no. 8, 2026. [doi:10.1109/JSEN.2026.3668906](https://doi.org/10.1109/JSEN.2026.3668906)
