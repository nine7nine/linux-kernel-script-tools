# linux-kernel-script-tools

This repo contains some very simple scripts or wrappers, mostly Linux-RT related.

* rtcqscan is a wrapper/downloader for the realtimeconfigquickscan.pl perl script. execute it in a folder (not /usr/bin).

* the cyc-hi/low scripts require cyclictest (for testing latency on rt-kernels). The cyc-hi script simulates 100% load on all cpu cores, while running cyclictest. In addition the scripts will reduce priority, after test benchmark is killed via CRTL-C, which gives an idea at different RT priorites what kind of latency you can expect. At the end it will also kill the simulated load.
 
* rtfifo checks rtirq status and also is a wrapper to check FIFO threads

* pcilat is for adjusting pci-latency

* procint is a wrapper for 'cat /proc/interrupts' in color.

* ghz is a wrapper for cpupower frequency-set. You type ghz + frequency. 3.4ghz, for example; 

$ ghz 3400
