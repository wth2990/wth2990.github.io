---
layout: post
title: "Lithography in microfluidics chip"
categories: misc
tags: Microfluidics
imageLink: "/assets/microfluidics/lithography/lithography_in_chip.png"
---
This was my master’s thesis, titled Microfluidic Stereolithography for Generating Cell Cultures with Spatial Order. The objectives of the project were:

1. to build an instrument for photolithography in microfluidics;
2. to perform photolithography within microfluidic channels;
3. to culture cells inside the microfluidic system.

The principle of photolithography in microfluidics is straightforward. A UV source is collimated by a convex lens, and the collimated UV light passes through a photomask that contains the desired 2D pattern. The UV light then illuminates the hydrogel precursor filled in the microfluidic channel through a glass substrate. The hydrogel polymerizes upon exposure to UV, forming a hydrogel pad with the designated shape. Subsequently, PBS solution or water is flushed through the channel to remove unpolymerized hydrogel precursors.

<p align="center">
  <img src="/assets/microfluidics/lithography/principle.jpeg" alt="principle" width="300">
  <br>
  <em>Figure 1: The principle of photolithography in microfluidics.</em>
</p>

## Instrument

The first stage of the project was to build the photolithography instrument, which was designed based on three main units: the imaging unit, the microfluidics unit, and the UV illumination unit.

The **imaging unit** enables observation during lithography and captures images or video. It consists of a CCD camera, lens tubes for magnification, and a white light source for illumination. The design of the imaging unit is shown below:

<p align="center">
  <img src="/assets/microfluidics/lithography/Image_Unit.png" alt="image unit" width="500">
  <br>
  <em>Figure 2: Imaging unit for observation and microscopy.</em>
</p>

The **microfluidics unit** is a static component designed to hold the microfluidic chips in place:

<p align="center">
  <img src="/assets/microfluidics/lithography/Microfluidic_Unit.png" alt="microfluidics unit" width="500">
  <br>
  <em>Figure 3: Microfluidics unit holding the chips.</em>
</p>

The **UV unit** provides UV illumination. It consists of a UV LED, a collimating lens, a 3D-printed photomask holder, and a 4-axis stage (X-Y-Z linear stages and a rotary stage):

<p align="center">
  <img src="/assets/microfluidics/lithography/UV_Unit.png" alt="uv unit" width="500">
  <br>
  <em>Figure 4: UV illumination unit.</em>
</p>

In addition to the mechanical components, the system includes electronics that control UV illumination via a Bluetooth receiver. Illumination parameters, including intensity and exposure time, are sent from a mobile device to the Bluetooth receiver. An Arduino processes the signals between the receiver and the UV LED:

<p align="center">
  <img src="/assets/microfluidics/lithography/Arduino.png" alt="arduino" width="800">
  <br>
  <em>Figure 5: Arduino-based control system for UV illumination.</em>
</p>

The figure below shows the assembled components, both as a schematic design and as the real instrument:

<p align="center">
  <img src="/assets/microfluidics/lithography/Insrtument concept and real.png" alt="instrument concept and real" width="500">
  <br>
  <em>Figure 6: Schematic design and real assembled instrument.</em>
</p>

The instrument operates in conjunction with an external PC for monitoring the microfluidic channels, and an external stage controller provided by Scientifica:

<p align="center">
  <img src="/assets/microfluidics/lithography/System_Schematic.png" alt="system schematic" width="800">
  <br>
  <em>Figure 7: Overall system schematic.</em>
</p>

## Microfluidics

Three microfluidic chips were designed:

* The **first chip** (left) is the simplest, consisting of 7 channels. Hydrogel polymerization occurs within the channels, serving to validate the principle of on-chip photolithography.
* The **second chip** (middle), designed by Stephen (a visiting PhD student), has 8 channels, each containing 8 round chambers with a central pillar. This chip was intended for cell culture using polymerized hydrogel, but the small channel dimensions limited its practical use.
* The **third chip** (right) is a modified version of Stephen’s design, with larger chambers and channels, as well as valves to control fluid flow. It was not used, as the first chip sufficed for the master thesis experiments, but it is intended for future applications.

<p align="center">
  <img src="/assets/microfluidics/lithography/MF_Chips.png" alt="microfluidic chips" width="300">
  <br>
  <em>Figure 8: Three designs of microfluidic chips.</em>
</p>

The microfluidic chips were fabricated via soft lithography. Pre-fabricated silicon wafers served as molds:

<p align="center">
  <img src="/assets/microfluidics/lithography/Wafer.png" alt="wafers" width="500">
  <br>
  <em>Figure 9: Silicon wafers used as molds for soft lithography.</em>
</p>

## Lithography on a Chip

Photomasks of varying shapes and sizes (800 µm to 30 µm) were designed to test the resolution of on-chip photolithography. The smallest achievable pattern was ~100 µm:

<p align="center">
  <img src="/assets/microfluidics/lithography/Mask_Holder_Photo.png" alt="mask variable size" width="300">
  <br>
  <em>Figure 17: Photomasks of varying shapes and sizes for resolution testing.</em>
</p>

Hydrogel pads with diamond shapes were stained with trypan blue for visualization, and excess dye was washed away with PBS:

<p align="center">
  <img src="/assets/microfluidics/lithography/Trypan_blue.png" alt="pattern on a chip" width="300">
  <br>
  <em>Figure 18: Diamond-shaped hydrogel pads stained with trypan blue.</em>
</p>

Resolution testing involved varying GelMA DoF and photo-initiator concentration. Higher photo-initiator concentration (1%) enabled formation of smaller features (14 patterns in 300 s), while lower concentration (0.5%) yielded only 10 patterns:

<p align="center">
  <img src="/assets/microfluidics/lithography/Pattern formed Result.png" alt="pattern form number result" width="500">
  <br>
  <em>Figure 19: Number of patterns formed vs. UV illumination time and photo-initiator concentration.</em>
</p>

Example hydrogel pads patterned in microfluidic channels. All channels were filled with PBS except the rightmost channel, which contained air:

<p align="center">
  <img src="/assets/microfluidics/lithography/lithography_in_chip.png" alt="cover picture" width="300">
  <br>
  <em>Figure 20: Hydrogel pads patterned in microfluidic channels.</em>
</p>

Some defects were observed: hydrogel pads deformed after flushing, likely due to swelling and fluid pressure:

<p align="center">
  <img src="/assets/microfluidics/lithography/flushing.png" alt="flushing comparison" width="300">
  <br>
  <em>Figure 21: Hydrogel pads deformed after flushing, likely due to swelling.</em>
</p>

Unwanted polymerization occurred, especially for concave shapes, likely due to UV scattering:

<p align="center">
  <img src="/assets/microfluidics/lithography/unwant_polymerization.png" alt="unwant polymerization" width="700">
  <br>
  <em>Figure 22: Unwanted polymerization observed, likely due to UV scattering.</em>
</p>

Patterns within channels were unevenly distributed, with central regions higher, likely because polymerization initiates from the center of the photomask holes:

<p align="center">
  <img src="/assets/microfluidics/lithography/uneven_distribution.png" alt="uneven distribution" width="700">
  <br>
  <em>Figure 23: Uneven distribution of hydrogel pads within channels; center regions higher than edges.</em>
</p>

<!--
This was my master’s thesis. The objectives of the project were:

1. to build an instrument for photolithography in microfluidics;
2. to perform photolithography within microfluidic channels;
3. to culture cells inside the microfluidic system.

The principle of photolithography in microfluidics is straightforward. A UV source is collimated by a convex lens, and the collimated UV light passes through a photomask that contains the desired 2D pattern. The UV light then illuminates the hydrogel precursor filled in the microfluidic channel through a glass substrate. The hydrogel polymerizes upon exposure to UV, forming a hydrogel pad with the designated shape. Subsequently, PBS solution or water is flushed through the channel to remove unpolymerized hydrogel precursors.

![principle](/assets/microfluidics/lithography/principle.jpeg){: width="300" }


## Instrument

The first stage of the project was to build the photolithography instrument, which was designed based on three main units: the imaging unit, the microfluidics unit, and the UV illumination unit.

The **imaging unit** enables observation during lithography and captures images or video. It consists of a CCD camera, lens tubes for magnification, and a white light source for illumination. The design of the imaging unit is shown below:

![image unit](/assets/microfluidics/lithography/Image_Unit.png){: width="500" }

The **microfluidics unit** is a static component designed to hold the microfluidic chips in place:

![microfluidics unit](/assets/microfluidics/lithography/Microfluidic_Unit.png){: width="500" }

The **UV unit** provides UV illumination. It consists of a UV LED, a collimating lens, a 3D-printed photomask holder, and a 4-axis stage (X-Y-Z linear stages and a rotary stage):

![uv unit](/assets/microfluidics/lithography/UV_Unit.png){: width="500" }

In addition to the mechanical components, the system includes electronics that control UV illumination via a Bluetooth receiver. Illumination parameters, including intensity and exposure time, are sent from a mobile device to the Bluetooth receiver. An Arduino processes the signals between the receiver and the UV LED:

![arduino](/assets/microfluidics/lithography/Arduino.png){: width="800" }

The figure below shows the assembled components, both as a schematic design and as the real instrument:

![instrument concept and real](/assets/microfluidics/lithography/Insrtument concept and real.png){: width="500" }

The instrument operates in conjunction with an external PC for monitoring the microfluidic channels, and an external stage controller provided by Scientifica:

![system schematic](/assets/microfluidics/lithography/System_Schematic.png){: width="800" }

## Microfluidics

Three microfluidic chips were designed:

* The **first chip** (left) is the simplest, consisting of 7 channels. Hydrogel polymerization occurs within the channels, serving to validate the principle of on-chip photolithography.
* The **second chip** (middle), designed by Stephen (a visiting PhD student), has 8 channels, each containing 8 round chambers with a central pillar. This chip was intended for cell culture using polymerized hydrogel, but the small channel dimensions limited its practical use.
* The **third chip** (right) is a modified version of Stephen’s design, with larger chambers and channels, as well as valves to control fluid flow. It was not used, as the first chip sufficed for the master thesis experiments, but it is intended for future applications.

![microfluidic chips](/assets/microfluidics/lithography/MF_Chips.png){: width="300" }

The microfluidic chips were fabricated via soft lithography. Pre-fabricated silicon wafers served as molds:

![wafers](/assets/microfluidics/lithography/Wafer.png){: width="500" }

## Hydrogels

Hydrogels are biocompatible materials used as the resin in photolithography on a chip. They are initially in liquid form and contain monomers with reactive double bonds. Upon exposure to a photo-initiator and UV light, the monomers polymerize in a chain reaction to form a crosslinked mesh structure, which can absorb water and swell.

For this work, I used photo-polymerizable gelatin methacryloyl (GelMA). One batch of GelMA takes approximately 7 days to synthesize. The procedure involves dissolving gelatin in water, adding methacrylic anhydride to graft methacryloyl groups onto the gelatin, and performing dialysis to remove unreacted methacrylic anhydride. The GelMA precursor is then freeze-dried for storage at -20°C:

![GelMA synthesis](/assets/microfluidics/lithography/photo_procedure_GelMA_Synthesis.png){: width="500" }

Mechanical properties of the hydrogel were characterized using a rheometer. Hydrogel pads were formed in PDMS molds and polymerized under UV light:

![hydrogel forming pad](/assets/microfluidics/lithography/photo_mechanical_test_mold.png){: width="300" }

The hydrogel pad was placed under the rheometer probe, which applied a ~1 N force while oscillating. The storage modulus reflects the material’s elastic response, while the loss modulus measures viscous behavior:

![rheometer measure](/assets/microfluidics/lithography/photo_rheometer_test.png){: width="500" }

The storage modulus was measured for GelMA batches with varying precursor concentrations. As expected, higher concentration yielded higher storage modulus:

![storage modulus](/assets/microfluidics/lithography/Result_2.png){: width="500" }

Plateau modulus (below 10 Hz) was stable and positively correlated with GelMA concentration:

![plateau modulus](/assets/microfluidics/lithography/Result_3.png){: width="500" }

The **degree of functionality (DoF)** quantifies the fraction of gelatin amine groups replaced by methacryloyl groups during grafting:

![schematic of DoF](/assets/microfluidics/lithography/DoF.png){: width="400" }

DoF was measured by ninhydrin assay for four GelMA batches with varying methacrylic anhydride content. All batches showed high DoF (>80%), indicating that even lower quantities of methacrylic anhydride are sufficient for GelMA synthesis:

![ninhydrin assay result](/assets/microfluidics/lithography/Result_1.png){: width="750" }

## Lithography on a Chip

Photomasks of varying shapes and sizes (800 µm to 30 µm) were designed to test the resolution of on-chip photolithography. The smallest achievable pattern was ~100 µm:

![mask variable size](/assets/microfluidics/lithography/Mask_Holder_Photo.png){: width="300" }

Hydrogel pads with diamond shapes were stained with trypan blue for visualization, and excess dye was washed away with PBS:

![pattern on a chip](/assets/microfluidics/lithography/Trypan_blue.png){: width="300" }

Resolution testing involved varying GelMA DoF and photo-initiator concentration. Higher photo-initiator concentration (1%) enabled formation of smaller features (14 patterns in 300 s), while lower concentration (0.5%) yielded only 10 patterns:

![pattern form number result](/assets/microfluidics/lithography/Pattern formed Result.png){: width="500" }

Example hydrogel pads patterned in microfluidic channels. All channels were filled with PBS except the rightmost channel, which contained air:

![cover picture](/assets/microfluidics/lithography/lithography_in_chip.png){: width="300" }

Some defects were observed: hydrogel pads deformed after flushing, likely due to swelling and fluid pressure:

![flushing comparison](/assets/microfluidics/lithography/flushing.png){: width="300" }

Unwanted polymerization occurred, especially for concave shapes, likely due to UV scattering:

![unwant polymerization](/assets/microfluidics/lithography/unwant_polymerization.png){: width="700" }

Patterns within channels were unevenly distributed, with central regions higher, likely because polymerization initiates from the center of the photomask holes:

![uneven distribution](/assets/microfluidics/lithography/uneven_distribution.png){: width="700" }

-->