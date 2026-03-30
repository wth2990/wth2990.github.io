---
layout: post
title: "Design microfluidics for particle separations"
categories: misc
tags: Microfluidics
imageLink: "/assets/microfluidics/particle_separation/DLD concepts.png"
date: 2025-07-05 22:30:00 +0200
---

My PhD thesis is titled “Development of Microfluidic Systems to Characterize Microbial Communities Trapped in Glacial Archives.” The core of my work focuses on using microfluidic chips to sort particles.

The background of this research lies in the fact that glacial meltwater contains a large number of microparticles, including various microorganisms such as bacteria and fungi. Analyzing these microorganisms can provide valuable insights into biological evolution, as many of them may have existed for thousands or even tens of thousands of years.

Conventional analysis methods typically rely on direct genomic sequencing of glacial meltwater samples. However, this approach may lack sensitivity, meaning that some rare taxa might not be detected. By contrast, microfluidic systems allow for pre-sorting of particles in the meltwater before sequencing. For example, particles can be categorized based on size: the smallest group may include bacteria (<1 µm), the next group fungi (3–5 µm), and larger particles such as dust (>10 µm). Sequencing each fraction separately can significantly improve detection accuracy, enabling the identification of rare taxa and providing a deeper understanding of low-abundance microbial populations in glacial environments.

It is worth noting that microbiological analysis is not my primary expertise; my specialization lies in the design and fabrication of microfluidic systems. In this project, we chose to use a deterministic lateral displacement (DLD) array as the microfluidic platform for particle sorting.


<!--![unwant polymerization](/assets/microfluidics/particle_separation/DLD concepts.png){: width="300" } <br> -->
<p align="center">
  <img src="/assets/microfluidics/particle_separation/DLD concepts.png" alt="unwant polymerization" width="300">
  <br>
  <span style="display:block; text-align:center;">
    Figure 1: The figure above illustrates the basic principle of the DLD array.
  </span>
</p>

The DLD approach offers several advantages:

1. It is a passive microfluidic system, requiring no external forces such as electric fields, magnetic fields, or acoustic waves, making it simple to operate without additional equipment.
2. It provides high sorting resolution, with studies demonstrating sub-micron precision.
3. It enables continuous sorting, ensuring a relatively high throughput.
4. Its design and fabrication are relatively straightforward and do not require highly complex processes.

During my PhD, I successfully fabricated DLD arrays capable of sorting 1 µm and 3 µm particles, and I validated their performance using microbeads. These results demonstrate that DLD is a reliable sorting technique. However, bead-based validation has its limitations, as beads are spherical, whereas real microorganisms can exhibit a variety of shapes, such as rod-like or elliptical forms.

DLD arrays also have certain drawbacks. For instance, they are prone to clogging. When processing large sample volumes or samples containing larger particles, direct introduction into the DLD array can lead to clogging. Once clogging occurs, the device may no longer be usable.

Due to the fact that related work has not yet been published, I have not presented all the results of my PhD research here. Once the associated publications are released, I will share my full findings, including aspects related to biological analysis.


<!--

这是我博士论文的题目，我的论文题目是《Development of microfluidic systems to characterize microbial communities trapped in glacial archives》，通过使用微流控芯片来sort particles。题目的背景是，在冰川融水里面有很多微颗粒，包括各种微生物，像是细菌或者fungi。然后分析这些微生物有助于我们了解生物进化，因为这些在冰川融水里的微生物很可能是数千年，甚至数万年以前的就已经存在着的生物。一般的分析方法，使用基因测序来直接分析冰川融水的样本，但是这样测序会有失精度，也就是一些rare taxa可能不会被测出。而如果使用微流控系统，先把冰川融水内的颗粒，先预分选，比如，按照颗粒大小把样本归类，最小颗粒的微生物分为一组（细菌 < 1 um)，次小的颗粒归为第二类（fungi 3-5um），然后最大的颗粒归为第三类（dust,>10um），如此类推。然后我们再按照每一组来测序，这样我们就会测得更准确的结果，一些rare taxa会被测出，有助于我们理解冰川融水内较为稀有得微生物。
上图就展示了DLD array的基本原理。
当然，分析微生物不是我的专项，我的专项是设计和制造微流控系统。这里我们选择使用了DLD array作为分选微生物的微流控芯片设计。因为DLD有几个好处，1. 它是被动的微流控，我们不需要额外地增加外力，像是电场、磁场、acoutic wave等等。使用起来比较简单，我们也不需要为它增添很多新的设备。2. 它可以有很高的sorting resolution，有人做过实验，它可以达到sub-micron级别的sorting resolution。3.它是continous sorting，这样可以确保我们的throughput不会太小。4.设计和制造工艺相对简单，不需要很多复杂的工艺。
然后在我的博士课题期间，我成功制造出可以分选1以及3um颗粒的DLD array，并且成功用bead演示过。这说明DLD是一个reliable的sorting技术。虽然，使用bead演示也有局限性，因为它是圆的，而实际上的微生物颗粒并不是完全圆的，有些是长条形的，或者椭圆形的等等。
当然，DLD sorting array也有一些drawback，比如它很容易clogging，如果我们有大量的样本，且比较大颗粒的样本，我们不可以直接导入DLD array里面，不然会clogging，一旦clogging，这片DLD array就不能再被使用了。
我这里没有完全地展示我在整个博士期间，制作DLD微流控芯片的结果，因为相关论文还没被发表。一旦发表，我就会在此展示我所做的结果，当中也涉及到一些生物学上的分析。

-->
