# linux-kernel-script-tools

This repo contains some very simple scripts or wrappers, mostly Linux-RT related.

* rtcqscan is a wrapper for the realtimeconfigquickscan.pl perl script, but additionally, will grad it from git [at execution].

* the cyc-* scripts require cyclictest (for testing latency on rt-kernels), however; the cyc-hi script also simulates loads on all cpu cores... In addition the scripts reduce priority, after CRTL-C is applied, which gives an idea at different RT priorites what kind of latency you can expect.
 
* rtfifo checks rtirq status and also is a wrapper to check FIFO threads

* pcilat is for adjusting pci-latency

* procint is a wrapper for 'cat /proc/interrupts' in color.
