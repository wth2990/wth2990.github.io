---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: page
---

# Introduction

Welcome to my website. My name is Tin Wang Wong. I am currently conducting research on microfluidics in France, and I am originally from Hong Kong. On these pages, you will find summaries of my past and ongoing research in the field of microfluidics, as well as topics that I am interested in.

In July 2025, I successfully defended my Ph.D. at the Université Grenoble Alpes (France), completing the degree in a total of three and a half years. Following this, in August 2025, I began working as a Research Engineer at the Institut de Physique de Nice in Nice, developing the Acoustofluidic Interferometric Device (AID). Starting June 2026, I will be joining the Soleil Synchrotron in Paris as a postdoctoral researcher.

Before my Ph.D., I obtained my Master’s degree in July 2018. My master’s thesis was titled “Microfluidic stereolithography for generating cell cultures with spatial order”. From October 2018 to June 2020, I worked as a microfluidics researcher at the Helmholtz Center in Munich, focusing on the development of hydrogel-based microfluidic devices.

I have experience with a range of microfluidic techniques, including acoustic microfluidics, DLD particle sorting, Microfluidic Large-Scale Integration (mLSI), and on-chip lithography. Below are detailed explanations:

## Acoustic Microfluidics

During my postdoctoral research, I used piezoceramics to generate acoustic waves that focused micro-particles within microfluidic channels. In other words, the particles flow only along the center of the channel. This setup involves electrical engineering aspects, as driving piezoceramics requires sufficient voltage (over 25 V) and current. It also requires a waveform generator capable of producing MHz-level signals and an amplifier to boost the generator’s output from millivolts or a few volts up to at least 25 V. If the amplifier’s power is insufficient, particles cannot be focused.

## DLD Particle Sorting

During my Ph.D., I developed DLD (Deterministic Lateral Displacement) microfluidic chips for particle sorting. Sorting means separating particles by size—larger particles move left, smaller particles move right. DLD is a passive sorting technique that does not rely on external forces or fields, such as electricity or magnetism. Although DLD was first developed in 2004 and is relatively mature, it can achieve nanometer-level sorting resolution. In my Ph.D. work at Liphy lab, I was able to fabricate DLD arrays capable of sorting 3 μm and 1 μm particles and used these arrays (together with related sister arrays) to separate fungi and bacteria.

## Microfluidic Fabrication

For any microfluidics developer, fabrication technology is always critical. I am familiar with several microfluidic fabrication techniques:
1. **Photolithography in cleanrooms**: I used SU-8 photoresist to create molds with micrometer-scale thicknesses, typically 50 μm in my Ph.D. work; 
2. **Soft lithography**: Using pre-fabricated silicon wafer molds, microfluidic channels are replicated in PDMS.; 
3. **3D printing**: While less precise than silicon wafers, 3D printing allows rapid prototyping. Using Cytop dip-coating, a non-stick layer can be added, enabling soft lithography replication of channels from 3D-printed molds; 
4. **Bioprinting**: Channels can also be printed using Pluronic F127, followed by molding or casting. After solidification, the chip is placed at 4°C to remove the Pluronic, leaving a hollow microfluidic channel.

These are the microfluidic fabrication techniques I have used in my research.

## Biological Techniques

I also have experience in cell culture and possess basic knowledge of cell cultivation techniques. I have previously cultured the HUVEC and HepG2 cell lines. In addition, I am capable of fabricating hydrogels; for example, I have prepared GelMA, a hydrogel that is polymerized using UV light.

<!-- 这是一个注释 

歡迎來到我的網頁。我叫Tin Wang Wong，目前在法國從事微流體研究，我來自香港。在這些頁面中，你會看到我曾經或正在研究的微流體領域的總結，以及我感興趣的相關內容。
我於2025年7月份在Université Grenoble Alpes成功答辯，並獲得博士學位，我一共花了3年半在攻读博士上。後來，2025年8月，我在尼斯的Institut de Physique de Nice任職research engineer，從事開發AID(Acoustofluidic Interferometric Device)。我将会在2026年6月在巴黎的Soleil synchrotron担任博士后研究员。
在博士前，我于2018年7月获得硕士学位，我的硕士论文是 “Microfluidic stereolithography for generating cell cultures with spatial order”。后来在2018年10月到2020年6月，我在慕尼黑的Helmholtz center担任微流控的研究员，从事hydrogel microfluidic的开发工作。

我所掌握的微流控技術包括，acoustic microfluidic, DLD particle sorting，Microfluidic large-scale integration （mLSI)，以及on-chip lithography。以下会详细解释：
Acoustic microfluidic:
我于我的博士后期间，使用piezoceramic来产生acoustic wave，从而使micro-particles在microfluidic中被focus，也就是说particles只在channel的最中央流动。当中涉及到一些电路的技术，因为驱动piezoceramic需要足够的电压（25V以上）与电流。这同时涉及到waveform generator以及amplifier。Waveform generator则需要达到能产生MHz级别的能力。而amplifier则需要把waveform generator产生的signal，从数Volt，或者mV，增强到至少25V，或者更高。如果amplifier的功率不足，particle是不能够被focus的。
DLD particle sorting:
我于博士期间开发过DLD microfluidic chip，用于sort particles。所谓的sort，就是把particle按大小归类，比如大的particle往左流动，小的往右。使用DLD的好处是可以passive sorting，就是说它不依赖external force或者媒介，比如不需要外接电源，外部磁场或电场等。DLD是一个比较老的技术，它从2004年被发明出来到现在已经有20多年。但是它却可以达到纳米级别的sorting resolution。对于我的博士期间，我能够利用我实验室(Liphy)的制造设备，制造出能sorting 3 um 和 1 um particles的DLD array，并且利用它(一起它的姐妹array)来分选fungi和bacteria。
Microfluidic fabrication:
与此同时，对于每一个microfluidic开发者来说，fabrication technology永远是重要的考量之一。我掌握一些不同的microfluidic fabrication technique，比如像是最传统的使用clean room的photo-lithography来制造mold。对此，我选用的photo resist是SU-8，它可以达到微米级别的厚度，当然，在我的博士论文中，我所选用的是50微米的厚度。另外，soft-lithography也是微流控的必备制造工艺。我们用这个技术，从事先制造好的silicon wafer mold中，把微流控的管道复制到PDMS上。
另外，我也有使用其他的方法来制造微流控device的经验。比如利用3D打印。3D打印的精度没有使用silicon wafer那么高，但是它可以快速prototype，以及制造出一些不需要很高精度的microfluidics。对于3D打印的microfluidics，我们也可以利用Cytop，把打印出来的塑料器件dip coating，从而附上一层防粘层。有了这一层防粘层，我们就可以使用soft-lithography，来把microfludic channel从3D打印出来的器件中，复制到PDMS上。
最后，值得一提的bio-printing。bio-printing也是一种fabrication technology。我们可以用bio-printing，把pluronic-F127打印成microfluidics的管道纹路。然后再用molding或者casting的技术制造microfluidics。一旦molding完成，倒模的材料从液体凝结成固体，我们就把microfluidic chip放到4度的环境中，在这低温环境中，pluronic-F127会从gel的状态变为液体，把这液体排除之后，然后我们就得到空的、成形的microfluidic channel。
以上几个方法，是我曾经使用过的microfluidci fabrication technologies。
Biological techniques:
我也曾經擁有cell culture的經驗，懂得一些基本的細胞培育的知識。我曾经培育过的细胞线有HUVEC和HepG2。另外，我也會fabricate hydrogel，我曾经制造过GelMA,一种使用UV来polymerise的hydrogel。

-->