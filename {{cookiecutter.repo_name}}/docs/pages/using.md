---
title: Using the Module
keywords: using
sidebar: manual_sidebar
permalink: using.html
summary: How to create designs using this module.
---

Using the {{site.product_name}} on a breadboard is easy: just connect the pins of the
module to the inputs of your circuitry wherever you need a pushbutton input.

If you're using the module to connect with one of the {{site.company_shortname}} FPGA boards
through a PMOD port, then the process is a bit more complicated:

 1. Create a Xilinx ISE/Vivado FPGA project and write some VHDL code for scanning the buttons.
 2. Attach the module to a PMOD socket on an {{site.company_shortname}} board.
 3. Determine the pins of the FPGA that connect to each I/O pin of the module.
 4. Make a UCF file associating each FPGA pin with an I/O pin of the module.
 5. Include the UCF file in your ISE/Vivado project and compile it into a bitstream.

That's a pretty big effort, so to get you started we've provided a 
[pre-built project]({{site.product_repo}}/tree/master/FPGA/ButtonTest) 
that you can modify for your own applications.

The pre-built project uses a specific PMOD port and {{site.company_shortname}} FPGA board.
To make it easier to move the module to another port or use a different board, 
we've built the [`xsconnect`](https://pypi.python.org/pypi/xsconnect) program that 
determines all the FPGA pin assignments for you.
For example, the image below shows the FPGA pin assignments for connecting the {{site.product_name}}
to the PM1 port of the {{site.stickit_mb}} V4.0 with a {{site.xula2}} FPGA board.
Just cut-and-paste the pin assignment constraints into the UCF file for your
project and you're good to go.

<img src="images/xsconnect.png" alt="Using the xsconnect program." style="width:100%;" class="center-it"/>



{% include links.html %}

