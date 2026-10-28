---
title: "In-hand pose estimation with vision and touch"
collection: portfolio
order: 4
period: "2020 – 2023"
venue: "IEEE Access"
thumb: inhand-thumb.jpg
thumb_alt: "Robot hand with two palm-mounted RGB cameras and two fingertip tactile sensors"
result: "Combining palm cameras with fingertip tactile sensors was more accurate than either alone; demonstrated pipette insertion into a transparent test tube."
paper: "https://doi.org/10.1109/ACCESS.2023.3244552"
video: "https://www.youtube.com/watch?v=2DNVzRrOgaw"
excerpt: "Estimating the 6D pose of a grasped object from two palm-mounted RGB cameras and two fingertip visuotactile sensors."
---

<figure class="fig">
  <img src="/images/research/inhand-overview.jpg" alt="Pipeline diagram and robot hand with two RGB cameras and two GelSight-type sensors">
  <figcaption>The pipeline, and the robot hand with two palm-mounted RGB cameras and two fingertip tactile sensors.</figcaption>
</figure>

**Goal.** Estimate the 6D pose of an object while the robot is holding it, without preparatory actions or special backgrounds, for objects made of a wide range of materials.

**Approach.** Two RGB cameras on the palm and two visuotactile sensors on the fingertips observe the grasped object from complementary viewpoints. Features from autoencoders trained on simulated images are matched against a pose database, coarse to fine, to estimate the object's 6D pose.

**Result.** With AR-marker ground truth on a 3D-printed object, combining cameras and touch was more accurate than camera-only or touch-only settings. The system was tested on five transparent, specular and metallic objects (15 trials each, placement deviation measured with a line laser) and used to insert a pipette into a transparent test tube.

**My role.** A laboratory team project with six authors; I am the first author. I built the fingertip sensors and mounted them on the hand, trained the networks and ran the estimation pipeline (the network code was written by a co-author), conducted all real-robot experiments and evaluation, and wrote the paper.

**Paper.** Y. Gao, S. Matsuoka, W. Wan, T. Kiyokawa, K. Koyama and K. Harada, "In-Hand Pose Estimation Using Hand-Mounted RGB Cameras and Visuotactile Sensors," *IEEE Access*, vol. 11, 2023. [doi:10.1109/ACCESS.2023.3244552](https://doi.org/10.1109/ACCESS.2023.3244552) · [Video](https://www.youtube.com/watch?v=2DNVzRrOgaw)
