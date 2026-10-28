---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="page__content">

<h2>Education</h2>

<div class="cv-entry"><span class="cv-what">Ph.D. in Engineering, The University of Osaka, Japan</span><span class="cv-when">Apr 2021 – Mar 2026</span></div>
<p class="cv-sub">Graduate School of Engineering Science, Department of Systems Innovation (Harada Lab). Supervisor: Prof. Kensuke Harada.</p>

<div class="cv-entry"><span class="cv-what">M.Eng., The University of Osaka, Japan</span><span class="cv-when">Apr 2019 – Mar 2021</span></div>
<p class="cv-sub">Same graduate school and department; research student there from Nov 2018 to Mar 2019.</p>

<div class="cv-entry"><span class="cv-what">B.Sc. in Physics, Zhejiang University, China</span><span class="cv-when">Sep 2014 – Jun 2018</span></div>
<p class="cv-sub">Chu Kochen Honors College, Qiushi Science Class (Physics).</p>

<h2>Research experience</h2>

<div class="cv-entry"><span class="cv-what">Miniaturization of vision-based tactile sensors (Ph.D. research)</span><span class="cv-when">2021 – 2026</span></div>
<p class="cv-sub">Lead researcher and first author of three journal papers. Part of the work was carried out under a JSPS bilateral program with Tsinghua University and Beijing University of Posts and Telecommunications.</p>
<ul class="cv-list">
  <li><strong>Folded optics and fluorescent illumination:</strong> 44 × 16 × 14 mm, parts about US$18. Optimized camera and mirror placement under field-of-view and occlusion constraints; replaced the three-color LED array with self-made fluorescent coatings excited by white LEDs.</li>
  <li><strong>Lensless pinhole imaging:</strong> thickness 34 → 15 mm against a lens-based setup with the same camera and field of view, guided by an imaging model of geometric blur, diffraction, refraction and field-of-view constraints.</li>
  <li><strong>Rotational scanning:</strong> field-of-view width 10 → 28 mm without increasing thickness, using a thin geared mechanism, rotation-center estimation (marker tracking, least squares, RANSAC) and center-weighted blending.</li>
  <li><strong>Calibration and evaluation:</strong> per-sensor color-to-gradient lookup tables, geometric calibration, Poisson integration; repeatability 0.063–0.097 mm; sharpness and texture metrics (Tenengrad, SSIM); identified the sources of reconstruction error.</li>
</ul>

<div class="cv-entry"><span class="cv-what">In-hand pose estimation with vision and touch</span><span class="cv-when">2020 – 2023</span></div>
<p class="cv-sub">Laboratory team project, six authors; first author.</p>
<ul class="cv-list">
  <li>Built the fingertip tactile sensors and integrated them with two palm-mounted RGB cameras; trained the networks and ran the estimation pipeline (network code by a co-author); conducted all real-robot experiments; wrote the paper.</li>
  <li>Camera and touch fusion was more accurate than either alone; demonstrated pipette insertion into a transparent test tube.</li>
</ul>

<p class="plain-links"><a href="/portfolio/">Project details →</a></p>

<h2>Publications</h2>

<p>Four peer-reviewed journal papers, all first-author: three in <em>IEEE Sensors Journal</em> (2024, 2025, 2026) and one in <em>IEEE Access</em> (2023). <a href="/publications/">Full list →</a></p>

<h2>Awards</h2>

<div class="cv-entry"><span class="cv-what">5th Excellent Research and Technology Award, The Robotics Society of Japan</span><span class="cv-when">2024</span></div>
<p class="cv-sub">First author; one of eight works selected that year. For the miniature tactile sensor research.</p>

<div class="cv-entry"><span class="cv-what">National runner-up, 7th China Undergraduate Physics Tournament (CUPT)</span><span class="cv-when">2016</span></div>
<p class="cv-sub">Zhejiang University team.</p>

<h2>Skills</h2>

<dl class="cv-dl">
  <dt>Optical modeling</dt>
  <dd>Imaging models (geometric blur, diffraction, refraction, field-of-view constraints), pinhole imaging, folded optics, fluorescent illumination, layout optimization.</dd>
  <dt>Calibration &amp; evaluation</dt>
  <dd>Photometric stereo, camera and fisheye calibration, AR-marker pose measurement, Tenengrad, SSIM, repeatability and error distributions.</dd>
  <dt>Image processing</dt>
  <dd>Python (NumPy, OpenCV), marker tracking, RANSAC, image registration and blending.</dd>
  <dt>Prototyping &amp; CAD</dt>
  <dd>Lens-removed CMOS cameras, pinhole fabrication and microscopy, silicone elastomers, reflective and fluorescent coatings, 3D printing, laser cutting, soldering; Onshape, Autodesk Inventor.</dd>
</dl>

<h2>Languages</h2>

<dl class="cv-dl">
  <dt>Chinese</dt>
  <dd>Native.</dd>
  <dt>Japanese</dt>
  <dd>JLPT N2 (2019). Studied and did research in Japan for more than seven years (2018–2026); reads and writes technical documents in Japanese.</dd>
  <dt>English</dt>
  <dd>TOEFL iBT 96 (2017). Wrote four first-author journal papers in English.</dd>
</dl>

<h2>Personal project</h2>

<div class="cv-entry"><span class="cv-what">Optimal-segment extraction from long gameplay recordings</span><span class="cv-when">2020 – 2022</span></div>
<p class="cv-sub">Planned and developed independently; coordinated about ten collaborators for two years.</p>
<ul class="cv-list">
  <li>Built an image-processing pipeline (digit segmentation, template matching, noise removal, time synchronization) to extract score curves from recordings; modeled the skill-activation rules and searched for their optimal combination.</li>
  <li>Covered 4,000+ charts (1,000+ songs × 4 difficulty levels) for 1,000+ users, with weekly updates.</li>
</ul>

</div>
