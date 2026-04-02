---
layout: post
title: "Create a lumen structure using bioprinting"
tags: Microfluidics
imageLink: "/assets/bioprinting/lumen_chip.jpeg"
---

This project was conducted after my master’s thesis, and its goal was to use bioprinting technology to create hydrogel lumen structures on a chip. The method is illustrated in the figure below. Before fabricating the chip, it is necessary to first create the PDMS surroundings, which I did using a 3D-printed mold. I will introduce this technology in another article.

<p align="center"> <img src="/assets/bioprinting/chip printing method.jpeg" alt="mask variable size" width="500"> <br> <em>Figure 1: Process of creating lumen structures using bioprinting.</em> </p>

According to the figure above, the first step is to coat a layer of hydrogel at the bottom and allow it to dry. Once it is dry, you can use a 3D printer to print your lumen structure on top of this hydrogel layer. The instrument used is a bioprinter, and the printing material is Pluronic F127. The Pluronic F127 used here is at a high concentration, which requires dissolving it in water using a centrifuge. I don’t recall the exact concentration, but it was around 50% or higher. At this high concentration, Pluronic F127 behaves like a gel.

After printing, the same hydrogel as the bottom layer is used to cast the upper part of the channel, essentially filling the PDMS surroundings with hydrogel. During casting, the hydrogel is still in liquid form, and it is then polymerized under specific conditions, such as at 37°C or using light. Once polymerized, you have an almost complete lumen structure within the microfluidic chip.

The next step is to remove the Pluronic F127 to reveal the lumen. To do this, the chip is placed in a refrigerator at 4°C. At this temperature, Pluronic F127 transitions from a gel to a liquid. You can then perfuse a liquid, such as water, through the lumen to flush out the Pluronic F127. This completes the creation of a usable lumen structure in hydrogel.

Finally, cells are seeded by introducing cell-containing culture medium into the lumen. This process is repeated for both sides. Afterward, you obtain a hydrogel lumen structure with cell-coated lumen walls, ready for further studies. The figure below shows the lumen after successfully removing the Pluronic F127.

<p align="center"> <img src="/assets/bioprinting/lumen_chip.jpeg" alt="mask variable size" width="300"> <br> <em>Figure 2: Lumen after flushing out Pluronic F127.</em> </p>

It is worth mentioning that the PDMS surroundings are clamped using a 3D-printed plastic holder. This holder, along with screws, provides a clamping force that seals the PDMS, preventing air from entering the surroundings (unless air permeates through the PDMS).

This sealing is important because the hydrogel lumen structure in the chip requires continuous perfusion for 24 hours. Without proper sealing, the culture medium from the external pump may not flow into the hydrogel lumen due to its relatively high resistance. Once sealed, the lumen forms a closed fluidic circuit with the external tubing, similar to a closed circuit in an electrical system, allowing fluid to flow from the external source into the lumen and then out.
{% comment %}
Might you have an include in your theme? Why not try it here!
{% include my-themes-great-include.html %}
{% endcomment %}

<!--
使用生物列印技術製作腔道結構

這個項目是在我碩士論文之後進行的，目標是使用生物列印技術在芯片上製作水凝膠腔道（lumen）。這個方法如下面的圖所示。在製作芯片之前，需要先製作 PDMS 的外殼（surroundings），我使用 3D 列印模具來完成這一步。我會在另一篇文章中介紹這項技術。

<p align="center">
  <img src="/assets/bioprinting/chip printing method.jpeg" alt="mask variable size" width="300">
  <br>
  <em>Figure 1: 使用生物列印技術製作腔道結構的過程.</em>
</p>

根據上圖，首先你要在最底層coat一層hydrogel，並且讓它風乾。乾了之後，你就可以用3D打印，在這一層hydrogel上打印你的lumen structure。你所使用的儀器是bioprinter，打印的材料是Pluronic F127，這裏所使用的Pluronic F127是高濃度的，需要使用離心機來讓它溶解在水中，具體濃度我不是太記得了，好像是50%，或更高。在高濃度的Pluronic F127情況下，它所呈現的是gel的質地。打印完之後，你就用和最底層一模一樣的hydrogel，來cast管道的上半部分，就是相當於把PDMS外殼用hydrogel填滿。當然，所謂的casting，就是你填充的時候，hydrogel還是液態，然後你把它放到一定的環境去polymerize，比如在37攝氏度的環境，或者用光來polymerize它。等它polymerize之後，你就有了一塊幾乎完成的lumen structure在microfluidics中，然後你的下一步就是要把Pluronic F127給移除掉，好讓lumen呈現出來。於是你把芯片放到零上四度的冰箱，在這個溫度下，Pluronic F127會從gel的狀態變成液體，然後你在lumen中perfuse液體，比如水，把液態的Pluronic F127給沖刷掉。這樣，可以用的lumen structure in hydrogel就完成了。最後就是seending cell，你把含有細胞的培養液導入lume中，放置一段時間，正反面都要重複一次，最後妳就有了可以用的lumen structure in hydrogel with cell coated lumen wall，你就可以進新對這個lumen的進一步研究。下圖是我成功在排空Pluronic F127後所呈現的管道。

<p align="center">
  <img src="/assets/bioprinting/lumen_chip.jpeg" alt="mask variable size" width="300">
  <br>
  <em>Figure 2: 在排空Pluronic F127後所呈現的管道.</em>
</p>

這裏要稍微提一下，這個PDMS外殼，是被用3D打印的塑料holder給夾著，這個holder，配上螺絲，提供了一個clamping force，這個clamping force可以把整個PDMS外殼密封化，就是外面的空氣不會流入外殼內部（除非空氣穿透PDMS）。因為，我這個lumen structure in hydrogel chip是需要24小時連續的perfusion的，所以這個密封性會很重要，如果不密封的話，我用外部pump的細胞培養液未必會流入這個hydrogel lumen內，因為這個hydrogel lumen會有比較強的阻力。所以，一旦密封了，整條lumen就會和外接的流體管道形成一個密閉的流體管道，相當於電路圖中的close circuit的概念，流體就得以從外部流入lumen，再從lumen流出。

{: width="250" }
-->