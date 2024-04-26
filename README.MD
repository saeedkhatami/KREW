# KREW: Kernel Read end(and) Write

A more stable & secure read/write virtual memory for kernel mode drivers

Intended to be called using Kernel Function hooks, but could be fitted to be used with **IOCTL**'s

These method's are slightly more secure compared to paracorded's methods (links in driver.c) and should be faster then **MmCopyVirtualMemory**

Created with the purpose of removing **PAGE_FAULT_IN_NONPAGED_AREA** bluescreen, and any other **BSOD**'s that come with copying bad memory
