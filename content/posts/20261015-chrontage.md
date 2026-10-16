---
title: "Chrontage"
date: 2026-10-15
description: "A Chronological Video Montage Maker"
cover:
  image: "images/vidclips.png"
  alt: "Placeholder image"
---

Years ago, on an old iPhone 6, I learned about a feature called "Memories" which took photos and videos on the device and made them into a chronological slideshows with background music.

I liked the feature and even used it a time or two to for little projects; however being the open source guy that I am, I wanted to figure out a way to make similar videos on GNU/Linux.  That took a long time.

Over the past couple of years I have searched for a way using bash scripts and other means with ffmpeg (a command line video editing tool) to get the results I wanted. But it really took exploring AI tools for programming before I began to have good results.

My latest and greatest script is called "Chrontage" and was the result of telling Grok (Xai) what I wanted. It took a couple of weeks of tinkering, but this little program, which consists of a short Bash script, a Python script, and a fonts folder, manages to make beautiful videos relying on only ffmpeg and Python3!

The following video was made completely offline from a folder full of unedited videos and a free audio track. I simply culled a few unwanted videoa and clips, made some minor adjustments and ran the script in my Termux (a free Linux terminal emulator for Android) and out came this video:

<div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/1236441178?badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share" referrerpolicy="strict-origin-when-cross-origin" style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Chrontage Test"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

I'll be sharing more on Chrontage in the near future.
