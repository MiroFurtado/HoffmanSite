---
title: "Hoffman Lab - SPSTM Intro"
layout: default
excerpt: "Hoffman Lab -- Spin-Polarized
Scanning Tunneling Microscopy"
sitemap: false
permalink: /research/SPSTMintro
---

# Spin-Polarized Scanning Tunneling Microscopy

A spin-polarized scanning tunneling microscopy (SP-STM) is an STM that is sensitive to the spin orientation of tunneling electrons. This allows us to make atomically resolved images of the magnetic order in a material.

Recall that an STM measures the local density of electronic states in a sample by tunneling through an atomically sharp tip positioned a few Ångstroms above the sample surface. The total tunneling current is proportional to the integrated density of states between the Fermi level and the relative tip-sample voltage.

$$
I \approx \frac { 4 \pi e } { \hbar } | M | ^ { 2 } \rho _ { T } ( 0 ) \int _ { - e V } ^ { 0 } \rho _ { S } ( \varepsilon ) \mathrm { d } \varepsilon
$$

A spin-polarized scanning tunneling microscope (SP-STM) employs much the same technique, but makes use of a magnetic tip to provide a source or sink of spin-polarized electrons for tunneling.

<table class="image" style="width: 300px; float: right; border: 10px">
<caption align="bottom" style="font-size:85%"><b>Fig. 1</b> Schematic of spin-polarized tunneling. Energy is along the vertical axis, while density of states of the tip and sample are on the horizontal axis. For spin ↓ electrons (green), there are many tip states for tunneling from, and many empty sample states for tunneling into. However, for spin ↑ electrons (blue), there are fewer tip states for tunneling from and fewer sample states for tunneling into. We measure the total tunneling current I↓ + I↑, and we assume that tunneling flips no spins.</caption>
<tr><td><img src="{{ site.url }}{{ site.baseurl }}/images/spstm_diagram.gif"/></td></tr>
</table>

We can think of the current as the sum of two separate spin channels, illustrated in Figure 1. To a good approximation, we assume that no electrons flip their spins while tunneling.

$$
I = I _ { \uparrow } + I _ { \uparrow } \propto \left| M ^ { 2 } \right| \int _ { - e V } ^ { 0 } \left[ \rho _ { S } ^ { \uparrow } ( \varepsilon - e V ) \rho ^ { \uparrow } _ { T } ( \varepsilon ) + \rho ^ { \downarrow } _ { S } ( \varepsilon - e V ) \rho ^ { \downarrow }_T ( \varepsilon ) \right] \mathrm { d } \varepsilon
$$

As in a traditional STM, $$ M  ^ 2$$ is the tunneling matrix element, and falls off exponentially with tip-sample distance. The spin-up density of states $$ρ^↑_T(ε)$$ refers to the number of spin-up states per unit energy and volume in the tip. If the tip DOS is approximately constant in the energy range of interest around the Fermi level, the SP-STM probes the local spin-polarized density of states in the sample.

We can define a quantity known as the spin-polarization of the tip or sample:

$$P = \frac { N _ { \uparrow } - N _ { \downarrow } } { N _ { \uparrow } + N _ { \downarrow } }$$

where 

$$
N _ { \uparrow } = \int _ { - e V } ^ { 0 } \rho ^ { \uparrow } ( \varepsilon ) \mathrm { d } \varepsilon
$$

P can range from 0 to 1. In Figure 1, for instance, $$P_T≈20%$$ and $$P_S≈90%$$. With this definition, the tunneling current can be expressed as

$$
I = I _ { 0 } \left( 1 + P _ { S } P _ { T } \cos \alpha \right) \equiv I _ { 0 } \left( 1 + \vec { P } _ { S } \cdot \vec { P } _ { T } \right)
$$

where $$I_0$$ is the spin-averaged current and α is the angle between the tip and sample magnetization, as shown in Figure 2. To get the best magnetic resolution, we want the tip and sample to be magnetized along the same axis.

<table class="image" style="width: 100px; float: right; border: 10px">
<caption align="bottom" style="font-size:85%"><b>Fig. 2</b> When magnetization axes of tip and sample are misaligned by an angle α, the tunneling current is proportional to (1+P_S P_T cosα).</caption>
<tr><td><img src="{{ site.url }}{{ site.baseurl }}/images/angle_diagram.gif"/></td></tr>
</table>

As with the density of states, spin polarization is a local quantity that may vary with position. If our sample is an antiferromagnet, $$P_S$$ will change direction with each unit cell. Imaging in constant current mode ("topographic" mode), this magnetic order causes an apparent difference in height, where "tall" atoms alternate with "short" ones. We can verify that the apparent modulation in height is due to magnetic order (and not some other effect) by changing the direction of the tip polarization.

If we instead image the differential conductance (dI/dV), the measured quantity is the energy-resolved spin polarization:

$$
P ( E ) \equiv \frac { \rho _ { \uparrow } ( E ) - \rho _ { \downarrow } ( E ) } { \rho _ { \uparrow } ( E ) + \rho _ { \downarrow } ( E ) }
$$

For some materials a $$dI/dV$$ map provides a stronger magnetic signal than topographic image.


To obtain spin-resolved images, we need a source of spin-polarized electrons. Specifically, we need the tip atom that is closest to the sample to have a well defined spin-polarization. Since exchange splitting causes spin-polarization in magnetic metals, the Hoffman lab will explore several options:
* Ferromagnetic materials, such as Nickel and Iron
* Antiferromagnets, such as Chromium and Manganese.
* A thin film of either a ferromagnet or antiferromagnet. Other labs have found that the preferred magnetization axis can depend on thickness of the film (<a href="https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.81.1495">see Wiesendanger, Rev Mod Phys 2009</a>).
* "Dunking" a nonmagnetic tip into a magnetic sample, to pick up a few spin-polarized atoms on the tip.


There are several trade-offs among these tip designs: ease of producing the tip, ability to stabilize, reproduce, and quantify the magnetization, ability to flip the magnetization with an applied field, and presence or absence of stray fields from the tip.





