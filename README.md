# linux-kernel-script-tools

This repo contains some very simple scripts or wrappers, mostly Linux-RT related.

* rtcqscan is a wrapper/downloader for the realtimeconfigquickscan.pl perl script. execute it in a folder (not /usr/bin).

* the cyc-hi/low scripts require cyclictest (for testing latency on rt-kernels). The cyc-hi script simulates 100% load on all cpu cores, while running cyclictest. In addition, the scripts will reduce priority after each test/benchmark is killed via CRTL-C. This helps to gives at different RT priority ranges, what kind of latency you can expect. At the end the script will kill  the simulated load.

cyclitest is a part of 'rt-tests' found here; https://git.kernel.org/cgit/utils/rt-tests/rt-tests.git/
 
* rtfifo checks rtirq status and also is a wrapper to check FIFO threads

* pcilat is for adjusting pci-latency

* procint is a wrapper for 'cat /proc/interrupts' in color.

* ghz - wrapper for cpupower frequency-set. You type ghz + frequency. 3.4ghz, for example; 

$ ghz 3400

* setcdl -  Simlpe script to adjust /dev/cpu_dma_latency manually. usage: 

$ setcdl (value in hexidecimal)

* pidaff - Check CPU affinity of a process and it's threads. usage:

$ pidaff foo (app/process name)

* cpuamap - script for creating a Cpu Affinity Map
