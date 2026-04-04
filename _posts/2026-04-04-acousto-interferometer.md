---
layout: post
title: "Acousto-interferometer device"
categories: microfluidics   # ⚠️ 必须小写并与 layout 中一致
tags: piezoceramic, Microfluidics
imageLink: "/assets/acousto_interferometer/chip_with_capillary.JPG"
---

I won’t go into too much detail because the instrument I am currently developing is patent-protected. Although I am not the patent holder, I signed a confidentiality agreement when I joined the company, so I cannot disclose the key technologies. However, I can give a brief overview since the underlying principles have already been published. I am not the first postdoc responsible for this project; before me, a PhD graduate also worked on developing this instrument.

First, there is a microfluidic channel—or in our case, we use a capillary. This microfluidic channel or capillary is attached to a piezoceramic device (piezo), which converts electrical signals into sound waves. The input electrical signal is generally a sinusoidal wave. 

We introduce particles into the microfluidic channel, using either a pressure pump or a syringe pump (personally, I prefer the pressure pump because it provides higher precision). Normally, under the flow of the fluid, particles are somewhat focused toward the center of the channel; this is called hydrodynamic focusing, though the focusing effect is not always optimal. 

If we turn on the piezo at this point, the sound waves interact with the particles and fluid, causing the particles to focus more precisely at the center of the channel. This is known as acoustic focusing.

Acoustic focusing not only keeps particles flowing along the center of the channel but also stretches them. Once particles are stretched, they produce interference under a laser, forming fringes. By analyzing the characteristics of these fringes, such as the number of fringe rings, we can determine the mechanical properties of the particles.

Of course, this project is currently at the development stage. Even at my current stage, I can only acquire partial data, so I have not yet been able to analyze it.

<!--
我不會說的太細緻，因為我現在開發的儀器是有專利保護的，雖然我不是專利的持有人，但是我在入職的時候也簽了保密協議，所以我不能披露其關鍵技術。但是我會稍微介紹一下其技術，因為其技術原理已經發表了。我不是第一個負責這個項目的博士後，在我之前，還有一個博士畢業生曾經負責開發這台儀器。
首先，會是有一個微流控管道，或者我們這裡是使用capillary。然後，這個微流控管道，或者capillary會attach一個piezoceramic device(piezo)，這個piezo會把電的訊號轉換成聲波。而輸入的電訊號一般是sinosodial wave。我們會把particles導入這個微流控管道，我們可以用pressure pump或者syringe pump，(其實我個人會是比較Prefer pressure pump，因為精度會大一點)。一般來說，particle在流體的驅動下，會某種程度被focus在管道的中間，我們說這是hydrodynamic focusing，但是它focus的效果未必是最好的。如果我們在這時turn on piezo，聲波傳送到particles和fluids，然後particles會被更好地focus在管道的中央。這就是所謂的acoustic focusing。
這個acoustic focusing除了可以讓particle只在管道的中央流動，也會stretch particles，particles被stretch之後，會在激光下產生interference，particle的話會形成fringe。通過分析fringe的質量，比如有多少個fringe ring等，我們可以知道particle的mechanical properties。
當然，這個項目，我現在只處於開發階段，甚至到我這一步，我只能acquire部分的data，所以我還沒能夠分析數據。
-->