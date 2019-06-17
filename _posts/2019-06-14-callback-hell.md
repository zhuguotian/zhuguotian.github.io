---
layout: post
title: Callback Hell
description: My personal understanding on callback functions and the ways javascript has developed to avoid it with arrow functions.
category: blog
---

## asynchronous(异步进程)
First from last semester OS course, we know that a program(程序) must include at least one process(进程), and one process must include at least on thread(线程).

<ul>
	<li>Program: a program is an executable file, e.g: chrome.exe, sublimetext.exe. Store at the secondary memory on computer(disk) and being read into primary memory.</li>
	<li>Process: a process is a executing instance of a program, e.g: if you double click on chrome icon, a chrome process is therefore created. One can have multiple process running on the primary memory and leave the memory if the system is ever rebooted. For example, if you happen to have the latest 1.5TB RAM apple laptop, you may be able to open two chrome processes :) </li>
	<li>Thread: a thread is the smallest excutable units of a process. e.g: when a program is started, the OS would start to execute the main thread of that process. Multiple thread can exist in one process, and each of those thread can do their own task. For example, a sublimetext process can have one thread reading the input while another thread saving the document. </li>
</ul>

After some basic concept, we know that usually a browser is multi-threaded, Javascript, on the other hand, is a [single threaded language][]. 

[single threaded language]: https://blog.csdn.net/baidu_24024601/article/details/51861792 "单线程分析"