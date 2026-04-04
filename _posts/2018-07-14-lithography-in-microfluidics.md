---
layout: post
title: "Lithography in microfluidics chip"
categories: microfluidics
tags: Microfluidics
imageLink: "/assets/microfluidics/lithography/lithography_in_chip.png"
---
This was my master’s thesis. The objectives of the project were:

1. to build an instrument for photolithography in microfluidics;
2. to perform photolithography within microfluidic channels;
3. characterize hydrogel
4. to culture cells inside the microfluidic system. However, this objective was not completed at the time I submitted my thesis.

In this article, I will introduce the first two points. The third point, regarding hydrogel, will be covered in the biotechnique section, where there is a dedicated article. The fourth point will not be discussed as it was not achieved.

The principle of photolithography in microfluidics is straightforward. A UV source is collimated by a convex lens, and the collimated UV light passes through a photomask that contains the desired 2D pattern. The UV light then illuminates the hydrogel precursor filled in the microfluidic channel through a glass substrate. The hydrogel polymerizes upon exposure to UV, forming a hydrogel structure with the designated shape. Subsequently, PBS solution or water is flushed through the channel to remove unpolymerized hydrogel precursors.

<p align="center">
  <img src="/assets/microfluidics/lithography/principle.jpeg" alt="principle of photolithography" width="300">
  <br>
  <em>Figure 1: Schematic illustration of the photolithography process in a microfluidic channel.</em>
</p>


## Instrument

The first stage of the project was to build the photolithography instrument, which was designed based on three main units: the imaging unit, the microfluidics unit, and the UV illumination unit. The **imaging unit** enables observation during lithography and captures images or video. It consists of a CCD camera, lens tubes for magnification, and a white light source for illumination. The **microfluidics unit** is a static component designed to hold the microfluidic chips in place. The **UV unit** provides UV illumination. It consists of a UV LED, a collimating lens, a 3D-printed photomask holder, and a 4-axis stage (X-Y-Z linear stages and a rotary stage).

In addition to the mechanical components, the system includes electronic control components that regulate UV illumination via a Bluetooth receiver. Illumination parameters, including intensity and exposure time, are sent from a mobile device to the Bluetooth receiver, and an Arduino processes the signals between the receiver and the UV LED. The figure below shows the assembled components, both as a schematic design and as the real instrument:

<p align="center">
  <img src="/assets/microfluidics/lithography/Insrtument concept and real.png" alt="instrument concept and real setup" width="500">
  <br>
  <em>Figure 2: Conceptual design and assembled photolithography instrument.</em>
</p>

The instrument operates in conjunction with an external PC for monitoring the microfluidic channels and is paired with a 3-axis external stage controller:

<p align="center">
  <img src="/assets/microfluidics/lithography/System_Schematic.png" alt="system schematic" width="800">
  <br>
  <em>Figure 3: System schematic showing integration of instrument, control, and monitoring components.</em>
</p>

## Microfluidics

Three microfluidic chips were designed:

* The **first chip** (left) is the simplest, consisting of 7 channels. Hydrogel polymerization occurs within the channels, serving to validate the principle of on-chip photolithography.
* The **second chip** (middle), designed by a visiting PhD student, has 8 channels, each containing 8 round chambers with a central pillar. This chip was intended for cell culture using polymerized hydrogel, but the small channel dimensions limited its practical use.
* The **third chip** (right) is a modified version of the visiting PhD student’s design, with larger chambers and channels, as well as valves to control fluid flow. It was not used in the master thesis experiments (as the first chip was sufficient), but it is intended for future applications. The images of these three microfluidic chips are shown below:

<p align="center">
  <img src="/assets/microfluidics/lithography/MF_Chips.png" alt="microfluidic chips" width="300">
  <br>
  <em>Figure 4: Three generations of microfluidic chip designs used for on-chip photolithography.</em>
</p>

## Lithography on a Chip

Photomasks of varying shapes and sizes (800 µm to 30 µm) were designed to test the resolution of on-chip photolithography. The smallest achievable pattern was ~100 µm.

Hydrogel structures with diamond shapes were stained with trypan blue for visualization, and excess dye was washed away with PBS:

<p align="center">
  <img src="/assets/microfluidics/lithography/Trypan_blue.png" alt="pattern on a chip" width="300">
  <br>
  <em>Figure 5: Diamond-shaped hydrogel patterns visualized using trypan blue staining.</em>
</p>

Resolution testing was conducted by varying the GelMA DoF and photo-initiator concentration. A higher photo-initiator concentration (1%) enabled the formation of smaller features (14 patterns in 300 s), while a lower concentration (0.5%) yielded only 10 patterns.

The following shows examples of hydrogel patterns formed in microfluidic channels. All channels were filled with PBS except the rightmost channel, which contained air:

<p align="center">
  <img src="/assets/microfluidics/lithography/lithography_in_chip.png" alt="hydrogel patterns in channels" width="300">
  <br>
  <em>Figure 6: Hydrogel patterns formed within microfluidic channels under different filling conditions.</em>
</p>

Some defects were observed: hydrogel structures deformed after flushing, likely due to swelling and fluid pressure:

<p align="center">
  <img src="/assets/microfluidics/lithography/flushing.png" alt="flushing comparison" width="300">
  <br>
  <em>Figure 7: Deformation of hydrogel patterns after հեղushing due to swelling and pressure effects.</em>
</p>

Unwanted polymerization occurred, especially for concave shapes, likely due to UV scattering:

<p align="center">
  <img src="/assets/microfluidics/lithography/unwant_polymerization.png" alt="unwanted polymerization" width="700">
  <br>
  <em>Figure 8: Unintended polymerization effects observed in concave geometries due to UV scattering.</em>
</p>

<!--
這是我的碩士論文。本專案的目標如下：

1. 建立一套用於微流體中的光刻儀器；
2. 在微流體通道內進行光刻；
3. characterize hydrogel
4. 在微流體系統中培養細胞。但是這一目標在我交論文的時候並沒有完成。

在這篇文章中，我會介紹前兩點。第三點，關於 hydrogel，我會放在 biotechnique 裡面，有專門文章介紹。第四點因為沒有做到，所以我不會對它介紹。

微流體中的光刻原理相當直接。UV 光源經由凸透鏡準直後，準直的 UV 光穿過包含所需 2D 圖案的光罩。接著，UV 光透過玻璃基板照射填充在微流體通道中的水凝膠前驅液。水凝膠在 UV 照射下發生聚合，形成具有指定形狀的水凝膠結構。隨後，使用 PBS 溶液或水沖洗通道，以去除未聚合的水凝膠前驅物。

![principle](/assets/microfluidics/lithography/principle.jpeg){: width="300" }

## Instrument

本專案的第一階段是建立光刻儀器，其設計基於三個主要單元：成像單元、微流體單元以及 UV 照明單元。

**成像單元（imaging unit）** 可在光刻過程中進行觀察並擷取影像或影片。它由 CCD 相機、用於放大的鏡筒以及白光光源組成。

**微流體單元（microfluidics unit）** 是一個靜態組件，用於固定微流體晶片的位置。

**UV 單元（UV unit）** 提供紫外光照明。它由 UV LED、準直透鏡、3D 列印的光罩固定器，以及一個四軸平台（X-Y-Z 線性平台與旋轉平台）組成。

除了機械元件外，系統還包含電子控制部分，透過藍牙接收器控制 UV 照明。照明參數（包括強度與曝光時間）由行動裝置傳送至藍牙接收器，並由 Arduino 在接收器與 UV LED 之間處理訊號。下圖展示了組裝後的元件，包括示意設計圖與實際儀器：

![instrument concept and real](/assets/microfluidics/lithography/Insrtument concept and real.png){: width="500" }

該儀器與外部電腦配合運作，用於監控微流體通道，並搭配了一個 3 axis 的外部平台控制器：

![system schematic](/assets/microfluidics/lithography/System_Schematic.png){: width="800" }

## Microfluidics

設計了三種微流體晶片：

* **第一種晶片**（左）最為簡單，由 7 條通道組成。水凝膠在通道內發生聚合，用於驗證晶片內光刻的原理。
* **第二種晶片**（中），由一個訪問博士生設計，具有 8 條通道，每條通道包含 8 個帶有中央柱的圓形腔室。該晶片原本用於利用聚合水凝膠進行細胞培養，但由於通道尺寸過小，實際應用受到限制。
* **第三種晶片**（右）是由此訪問博士生的改良版本，具有更大的腔室與通道，並加入閥門以控制流體流動。該晶片在本碩士論文實驗中未被使用（因第一種晶片已足夠），但預計用於未來應用。這三種微流體晶片的圖片為：

![microfluidic chips](/assets/microfluidics/lithography/MF_Chips.png){: width="300" }

## Lithography on a Chip

設計了不同形狀與尺寸（800 µm 至 30 µm）的光罩，以測試晶片內光刻的解析度。最小可達圖案約為 ~100 µm。

菱形水凝膠結構使用台盼藍染色以利觀察，並以 PBS 洗去多餘染料：

![pattern on a chip](/assets/microfluidics/lithography/Trypan_blue.png){: width="300" }

解析度測試透過改變 GelMA 的 DoF 與光引發劑濃度進行。較高的光引發劑濃度（1%）可形成較小特徵（300 秒內形成 14 個圖案），而較低濃度（0.5%）僅形成 10 個圖案。

以下為在微流體通道中形成的水凝膠圖案範例。所有通道均填充 PBS，唯最右側通道為空氣：

![cover picture](/assets/microfluidics/lithography/lithography_in_chip.png){: width="300" }

觀察到一些缺陷：水凝膠在沖洗後發生變形，可能是由於膨脹與流體壓力所致：

![flushing comparison](/assets/microfluidics/lithography/flushing.png){: width="300" }

出現非預期的聚合現象，特別是在凹形圖案中，可能是由於 UV 散射造成：

![unwant polymerization](/assets/microfluidics/lithography/unwant_polymerization.png){: width="700" }

-->