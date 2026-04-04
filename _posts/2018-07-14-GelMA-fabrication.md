---
layout: post
title: "GelMA fabrication and characterization"
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


<!--
## Hydrogels

水凝膠是一種生物相容性材料，在晶片光刻中作為樹脂使用。它們最初為液態，並含有具有反應性雙鍵的單體。在光引發劑與紫外光的作用下，這些單體會透過鏈式反應進行聚合，形成交聯的網狀結構，該結構可以吸收水分並發生膨脹。

在本研究中，我使用了可光聚合的明膠甲基丙烯醯（GelMA）。每一批 GelMA 的合成大約需要 7 天。其製備流程包括：將明膠溶於水中，加入甲基丙烯酸酐，使甲基丙烯醯基接枝到明膠分子上，並透過透析去除未反應的甲基丙烯酸酐。之後將 GelMA 前驅物進行冷凍乾燥，並儲存在 -20°C：

<p align="center">
  <img src="/assets/microfluidics/lithography/photo_procedure_GelMA_Synthesis.png" alt="GelMA synthesis" width="500">
  <br>
  <em>Figure 1：GelMA 的合成流程。</em>
</p>

水凝膠薄片在 PDMS 模具中形成，並在紫外光下進行聚合：

<p align="center">
  <img src="/assets/microfluidics/lithography/photo_mechanical_test_mold.png" alt="hydrogel forming pad" width="300">
  <br>
  <em>Figure 2：在 PDMS 模具中形成的水凝膠薄片。</em>
</p>

水凝膠的機械性質透過流變儀進行表徵：

<p align="center">
  <img src="/assets/microfluidics/lithography/photo_rheometer_test.png" alt="rheometer measure" width="500">
  <br>
  <em>Figure 3：用於測量儲能模數與損耗模數的流變儀實驗設置。</em>
</p>

對不同前驅物濃度的 GelMA 批次測量其儲能模數。結果如預期，濃度越高，儲能模數越大：

<p align="center">
  <img src="/assets/microfluidics/lithography/Result_2.png" alt="storage modulus" width="500">
  <br>
  <em>Figure 4：不同濃度 GelMA 水凝膠的儲能模數。</em>
</p>

平台模數（10 Hz 以下）保持穩定，並與 GelMA 濃度呈正相關：

<p align="center">
  <img src="/assets/microfluidics/lithography/Result_3.png" alt="plateau modulus" width="500">
  <br>
  <em>Figure 5：10 Hz 以下頻率範圍內 GelMA 的平台模數。</em>
</p>

**官能化程度（DoF）** 用於量化在接枝過程中，明膠中的胺基被甲基丙烯醯基取代的比例：

<p align="center">
  <img src="/assets/microfluidics/lithography/DoF.png" alt="schematic of DoF" width="400">
  <br>
  <em>Figure 6：GelMA 官能化程度（DoF）的示意圖。</em>
</p>

透過茚三酮測試（ninhydrin assay）測量四批不同甲基丙烯酸酐含量的 GelMA，其結果顯示所有批次均具有較高的 DoF（>80%）：

<p align="center">
  <img src="/assets/microfluidics/lithography/Result_1.png" alt="ninhydrin assay result" width="750">
  <br>
  <em>Figure 7：茚三酮測試結果顯示所有 GelMA 批次均具有高 DoF。</em>
</p>
-->