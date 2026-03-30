---
layout: post
title: "GelMA fabrication"
categories: biotechnique   # ⚠️ 必须小写并与 layout 中一致
tags: GelMA, hydrogel
imageLink: "/assets/microfluidics/lithography/photo_procedure_GelMA_Synthesis.png"
---

## Hydrogels

Hydrogels are biocompatible materials used as the resin in photolithography on a chip. They are initially in liquid form and contain monomers with reactive double bonds. Upon exposure to a photo-initiator and UV light, the monomers polymerize in a chain reaction to form a crosslinked mesh structure, which can absorb water and swell.

For this work, I used photo-polymerizable gelatin methacryloyl (GelMA). One batch of GelMA takes approximately 7 days to synthesize. The procedure involves dissolving gelatin in water, adding methacrylic anhydride to graft methacryloyl groups onto the gelatin, and performing dialysis to remove unreacted methacrylic anhydride. The GelMA precursor is then freeze-dried for storage at -20°C:

<p align="center">
  <img src="/assets/microfluidics/lithography/photo_procedure_GelMA_Synthesis.png" alt="GelMA synthesis" width="500">
  <br>
  <em>Figure 1: GelMA synthesis procedure.</em>
</p>

Hydrogel pads were formed in PDMS molds and polymerized under UV light:

<p align="center">
  <img src="/assets/microfluidics/lithography/photo_mechanical_test_mold.png" alt="hydrogel forming pad" width="300">
  <br>
  <em>Figure 2: Hydrogel pad formed in PDMS mold.</em>
</p>

Mechanical properties of the hydrogel were characterized using a rheometer:

<p align="center">
  <img src="/assets/microfluidics/lithography/photo_rheometer_test.png" alt="rheometer measure" width="500">
  <br>
  <em>Figure 3: Rheometer measurement setup for storage and loss modulus.</em>
</p>

The storage modulus was measured for GelMA batches with varying precursor concentrations. As expected, higher concentration yielded higher storage modulus:

<p align="center">
  <img src="/assets/microfluidics/lithography/Result_2.png" alt="storage modulus" width="500">
  <br>
  <em>Figure 4: Storage modulus of GelMA hydrogels with different concentrations.</em>
</p>

Plateau modulus (below 10 Hz) was stable and positively correlated with GelMA concentration:

<p align="center">
  <img src="/assets/microfluidics/lithography/Result_3.png" alt="plateau modulus" width="500">
  <br>
  <em>Figure 5: Plateau modulus of GelMA at frequencies below 10 Hz.</em>
</p>

The **degree of functionality (DoF)** quantifies the fraction of gelatin amine groups replaced by methacryloyl groups during grafting:

<p align="center">
  <img src="/assets/microfluidics/lithography/DoF.png" alt="schematic of DoF" width="400">
  <br>
  <em>Figure 6: Schematic of GelMA degree of functionality (DoF).</em>
</p>

DoF was measured by ninhydrin assay for four GelMA batches with varying methacrylic anhydride content. All batches showed high DoF (>80%):

<p align="center">
  <img src="/assets/microfluidics/lithography/Result_1.png" alt="ninhydrin assay result" width="750">
  <br>
  <em>Figure 7: Ninhydrin assay results showing high DoF for all GelMA batches.</em>
</p>


