---
title: Operation
keywords: operation
sidebar: manual_sidebar
permalink: operation.html
summary: Basic theory of operation of this module.
---

All eight buttons of the {{site.product_name}} are built from the following circuit:

<img src="images/circuit.png" alt="Basic circuit for the {{site.product_name}}." style="width:50%;" class="center-it"/>

When a pushbutton is pressed, the corresponding pin on the PMOD and breadboard
headers is pulled to ground through the 4.7 K&Omega; resistor.
When the pushbutton is released, the pin is pulled to the voltage applied to the
VCC pin of the module through a combined resistance of 5 K&Omega;.

There is no hardware debouncing of the switches.
Why? Because you can't have everything, so just live with it.



{% include links.html %}

