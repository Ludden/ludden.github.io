---
layout: post
title: When Virtualbox hangs in guru meditation
---

When a Virtualbox VM crashes due to insufficient resources it can sometimes go into a state of 'Guru meditation' and the UI controls won't allow to even shut it down.

This will usually do the trick:

~~~
VBoxManage list vms
VBoxManage controlvm "VM NAME" poweroff
~~~
