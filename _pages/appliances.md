---
layout: page
title: Appliances
permalink: /vm/
description:
redirect:
nav: false
nav_order: 100
---

I have created a virtual appliance for students to use to practice and do exams on. This appliance can also be used for other courses with minimal or no modifications and therefore students are free to install or modify it to suit their needs. Account passwords match the account names.

**Note:** This VM does not cover all of my courses. At the time of development, it supported: Object-Oriented Programming, Programming Paradigms, Computer Networks and Functional Programming.

The latest version: v1.1 (March 2021):
- [[.vmx](https://drive.google.com/file/d/1EnQD73tmLmXhp2vnyJZ5rfT1ydRYRwap/view?usp=sharing)]
[[.sha512](/assets/sha/irvm_v1.sha512)]
(portable, VMware)
- [[.ovf](https://drive.google.com/file/d/1eq1j3D8yD9V8kHOi5dM4KBql4dEDqlZk/view?usp=sharing)]
[[.sha512](/assets/sha/irvm_v1_ovf.sha512)]
(importable, VMware | VirtualBox)

### Patch notes
#### v1.1
- Added PyCharm on request

### Troubleshooting
- Make sure that the VM is properly downloaded and extracted.
- When running the VM for the first time, make sure to select the "I copied it" option when prompted with a VM migration question.
- If using VMware and the VM boots to a black screen, make sure that the Display settings in the VMware VM settings tab have the following:
  - Accelerated 3D graphics is enabled
  - VRAM is set to atleast 512MB
- Booting the display using an alternative, lightweight window manager is also possible, and can be used as a last-resort method if everything else fails. Use `Ctrl + Alt + F2` to open the text terminal. Login with the `user` account credentials (password matches the user name). Run `startx` to start the alternative window manager.
