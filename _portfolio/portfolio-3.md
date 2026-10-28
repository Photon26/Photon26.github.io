---
title: "Folded optics and fluorescent illumination"
collection: portfolio
order: 3
period: "2024"
venue: "IEEE Sensors Journal · RSJ Award"
thumb: miniature-thumb.jpg
thumb_alt: "Miniature tactile sensor held between two fingers"
result: "44 × 16 × 14 mm, parts about US$18, small enough to mount two on a parallel gripper."
paper: "https://doi.org/10.1109/JSEN.2024.3452768"
excerpt: "A miniature photometric vision-based tactile sensor built with optimized folded optics and fluorescent illumination, 44 × 16 × 14 mm."
---

<figure class="fig">
  <img src="/images/research/miniature-overview.jpg" alt="Miniature tactile sensor in hand, its exploded design, dimensions, and two sensors on a gripper">
  <figcaption>The sensor in hand, its components (a, b), dimensions (c), and two sensors on a parallel gripper (d).</figcaption>
</figure>

**Problem.** Vision-based tactile sensors give high-resolution contact geometry, but they are usually too large for compact grippers. Photometric stereo also needs light from three directions in three colors, which normally means a three-color LED array.

**Approach.** I formulated the placement of the camera and mirror as an optimization problem, constrained by the required field of view and by occlusion of the light path, and solved it numerically. For illumination, I painted self-made fluorescent coatings on three sides of an acrylic light guide and excited them with white LEDs, which removed the LED array and cut the width from 20 mm to 16 mm. Per-sensor color-to-gradient lookup tables, built from reference-sphere indentation, absorb the differences in fluorescent intensity between sensors.

**Result.** A 44 × 16 × 14 mm sensor with parts costing about US$18. Two of them on a two-finger parallel gripper reconstructed depth maps of the contact surface, and comparisons against variants with different lighting, camera and mirror setups showed what each component contributes.

**Recognition.** This work received the 5th Excellent Research and Technology Award of The Robotics Society of Japan (2024), one of eight works selected that year.

**My role.** Lead researcher and first author: optimization, optical and mechanical design, coatings and prototyping, calibration, experiments and writing.

**Paper.** Y. Gao, S. Zhang, W. Wan, B. Fang, F. Sun and K. Harada, "Development of a Miniature Photometric Vision-Based Tactile Sensor," *IEEE Sensors Journal*, vol. 24, no. 20, 2024. [doi:10.1109/JSEN.2024.3452768](https://doi.org/10.1109/JSEN.2024.3452768)
