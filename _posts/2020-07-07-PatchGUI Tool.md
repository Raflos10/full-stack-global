---
layout: post
author: Andrew
title: PatchGUI Tool
categories: software-projects
---

A cross-platform GUI application for creating and applying patches to binary files.

[Github Page](https://github.com/Raflos10/PatchGUI)

<figure class="w-full max-w-2xl mx-auto my-8">
  <video controls class="w-full rounded-lg shadow-md">
    <source src="/assets/videos/2020-07-07-11-26-27.mp4" type="video/mp4">
  </video>
</figure>

PatchGUI Tool Demonstration

- This software is built using Qt Creator 5, and the bsdiff library.
- Runs on Linux in the video, but can also be compiled for Windows or Mac

The main use-case for this software is to generate update files that are vastly smaller and faster to download than entirely new files. These patch files can be generated and applied using this tool, or they can be generated with this tool, distributed to users, and applied using an update software that includes the bsdiff library. This makes downloading updates for applications much faster and take up much less space.

By using suffix sorting (specifically, Larsson and Sadakane’s qsufsort) and taking advantage of how executable files change, bsdiff routinely produces binary patches 50-80% smaller than those produced by Xdelta, and 15% smaller than those produced by .RTPatch (a $2750/seat commercial patch tool).

Bsdiff runs in O((n+m) log n) time; on a 200MHz Pentium Pro, building a binary patch for a 4MB file takes about 90 seconds. bspatch runs in O(n+m) time; on the same machine, applying that patch takes about two seconds.
