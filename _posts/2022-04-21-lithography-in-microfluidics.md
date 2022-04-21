---
layout: post
title: "Lithography in microfluidics chip"
categories: misc
tags: Microfluidics
imageLink: "/assets/microfluidics/lithography/lithography_in_chip.png"
---

This was my master thesis. The target of the project is 1) to build an instrument for photo-lithography in microfluidics; 2) to make photo-lithographies inside microfluidics; 3) to culture cell within microfluidics.

## Instrument

The first stage is to build an instrument for photo-lithography. This instrument was built based on ... . There are three units: image unit, microfluidics unit, and UV unit.

The image unit is for taking video/images, and observation during lithography. It consists of a CCD camera, lens tubes, which were for amplification, and a white light source, which served as an illumination for microscopy. The design of the image unit is shown below.

![image unit](/assets/microfluidics/lithography/Image_Unit.png){: width="500" }

<br>
<br>

The microfluidics unit is for holding microfluidics. It is solely a static component.

![microfluidics unit](/assets/microfluidics/lithography/Microfluidic_Unit.png){: width="500" }

<br>
<br>

The UV unit is for illuminating UVs. There are UV LED, lens which collimates UV light, and a photomask holder, which was 3D printed and for holding a photomask, and a 4-axis stage, x-y-z stage and a rotatory stage.

![uv unit](/assets/microfluidics/lithography/UV_Unit.png){: width="500" }

<br>
<br>

Beside to mechanical parts, there is also electronics, which controls UV illuminations with an bluetooth receiver. So the illumination command, including the intensity and time, was sent by a mobile device, which was connecting to the bluetooth receiver. An Arduino was used for processing the signals in between bluetooth receiver and UV LED.

![arduino](/assets/microfluidics/lithography/Arduino.png){: width="800" }

<br>
<br>

By the way, this figure shows all the assembled components, in schematic design and real instrument.

![instrument concept and real](/assets/microfluidics/lithography/Insrtument concept and real.png){: width="500" }

<br>
<br>

The instrument is not supposed to work independently, but also with an external PC, which observes the situation in microfluidics, and an external stage controller, which was provided by scientifica.

![system schematic](/assets/microfluidics/lithography/System_Schematic.png){: width="800" }

<br>
<br>

## Microfluidics

Three microfluidic chips were designed. The first chip (left) is mostly used, and simplest among all. It consists of only 7 channels. So the hydrogel can be polymerized within the channel. This chip is to prove the principle of photo-lithography on a chip.

The second chip (middle) is designed by Stephen, who were the visiting PhD student. There are 8 channels. Each channel consists 8 round chambers, and in the center of each chamber there is a round pillar. This chip is designed for creating cell cultures using polymerized hydrogel in each chamber. In the end, it is not utilized widely, because the dimension of the channels is too small, which is not facilitating the polymerization on a chip.

The third chip (right) is a modified version toward the Stephen's chip. It has larger chamber and channel size. It has also the valves, which controls the close or open of the microfluidic channel. It is not used, because the first chip is enough to handle all the experiments for my master thesis, and it is supposed to be used for future...

![microfluidic chips](/assets/microfluidics/lithography/MF_Chips.png){: width="500" }

<br>
<br>

Microfluidics was fabricated via soft-lithography. A silicon wafer will be pre-fabricated, which served as a mold. The figure below displays the wafers used for fabricating the chips above.

![wafers](/assets/microfluidics/lithography/Wafer.png){: width="500" }

## Hydrogels

Hydrogel is a bio-compatible material. Which is used as the resin for photolithography on a chip. Normally, the hydrogel is fabricated in liquid state, which consists of lots of monomer, which has vast double bonds. Once the photo-initiator react with the monomer, it starts to form polymer with other monomers. And it is a chain reaction, therefore, a very long polymer could be formed in the end. Many polymers form meshwork structures, which was the essence of polymerized hydrogel. The polymerized hydrogel can be absorbed by water, that was called swelled state.

Here I have used the photo-polymerizable hydrogel, which modified from gelatin, called Gelatin methacryloyl (GelMA), for the photo-lithography experiments. It takes 7 days to fabricate one batch of GelMA. Basically, the fabricating procedure is to dissolve gelatin into water, add methacryloyl into gelatin solution, a chemical phenomenon called "graft" will happen, that will replace the amine group originally within gelatin molecules, and then dialysis the 7 days. The dialysis is to remove the unreacted methacryloyl, which is toxic. The dialysis is shown in the left figure below. For better storage, the GelMA precusory will be freeze-dried. The middle figure is shown the freeze-dried GelMA. The right figure shows the way to store the GelMA, which was frozen under -20&#176;C.

![GelMA synthesis](/assets/microfluidics/lithography/photo_procedure_GelMA_Synthesis.png){: width="500" }

<br><br>


I used rheometer to characterize its mechanical property, specifically the storage and loss modulus.

![rheometer measure](/assets/microfluidics/lithography/photo_rheometer_test.png){: width="500" }

## Lithography on a chip
