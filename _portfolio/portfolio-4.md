---
title: "Lensless pinhole imaging for a thinner sensor"
collection: portfolio
order: 2
period: "2025"
venue: "IEEE Sensors Journal"
thumb: pinhole-thumb.jpg
thumb_alt: "Pinhole tactile sensor held between two fingers"
result: "Thickness 34 → 15 mm against a lens-based design with the same camera and field of view."
paper: "https://doi.org/10.1109/JSEN.2025.3604943"
excerpt: "A vision-based tactile sensor that images through a pinhole instead of a lens, reducing thickness from 34 mm to 15 mm."
---

<figure class="fig">
  <img src="/images/research/pinhole-overview.jpg" alt="Pinhole tactile sensor, its exploded view, and the imaging geometry">
  <figcaption>The prototype and its components, the exploded design (a), and the imaging geometry used in the model (b).</figcaption>
</figure>

**Problem.** In a camera-based tactile sensor, the lens assembly sets a lower bound on thickness.

**Approach.** I replaced the lens with a pinhole and built an imaging model covering geometric blur, Fraunhofer diffraction, the effective thickness of the pinhole, refraction, and field-of-view constraints, then solved for the minimum thickness in Python. The prototype uses a commercial camera with its lens removed. I measured the aperture under a microscope (0.083 mm), back-calculated the effective pinhole thickness (0.081 mm) from the projected spot, and fed it back into the model to fix the final structure.

**Result.** Thickness dropped from 34 mm to 15 mm compared with a fisheye-lens setup using the same camera and the same field of view. Repeatability: pressing a sphere, a screw and a wrench ten times each gave mean per-pixel depth standard deviations of 0.063–0.097 mm. Sharpness was evaluated with Tenengrad and the high-frequency energy ratio. The price of a pinhole is less light and therefore lower contrast; the evaluation also identified non-uniform illumination as the source of errors around the contact region.

**My role.** Lead researcher and first author: imaging model and analysis, design, prototyping, calibration, evaluation and writing.

**Paper.** Y. Gao, S. Zhang, W. Wan, B. Fang, F. Sun and K. Harada, "Development of a Compact Tactile Sensor Using a Pinhole RGB Camera," *IEEE Sensors Journal*, vol. 25, no. 19, 2025. [doi:10.1109/JSEN.2025.3604943](https://doi.org/10.1109/JSEN.2025.3604943)
