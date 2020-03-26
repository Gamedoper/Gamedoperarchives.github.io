---
layout: post
title:  "DOOM Eternal Loading Screen Crash / Error Fix"
author: Gamedoper
categories: [GAMEERRORFIX]
image: https://i.imgur.com/pkQmIdp.jpg
tags: [featured]
---

# DOOM **Eternal**  FIX FOR LEVEL LOADING SCREEN CRASH
  

![e](https://i.imgur.com/9WNcuB0.jpg)

**DOOM Eternal is a pretty good game but it has some problems** , Especially on PC There is currently a problem with the game on the loading screen of the scenarios that is present on certain computers without an apparent reason.

**The video game crashes on the loading screen** , preventing it from playing normally. There is no patch to solve this problem, which can be a headache for many players.

Found a Solution on Doom Eternal Steam Page which seems to be working for many. 


### The steps are the following:

-   Open the game's command console by pressing the tilde key (the key that seems ~)
-   Write "logFile 2"

![enter image description here](https://i.imgur.com/USfxHpi.jpg)

- This will allow the console logs to be saved to disk. **Just writing this code solves the blessed crash on the loading screen.**

- This will enable console logs to be saved on disk.
- If you're having low FPS after the level successfully loads, consider doing "logFile 0" right after the level starts. Some people in this thread have reported that FPS gets fixed after that.

**The "logFile 2" command seems to clear the game buffer** every time logs are printed or written to disk, which could have prevented the sequence crash that occurs on the loading screen.

We can't guarantee this will work for everyone, but it seems to work from the comments on the [Steam](https://steamcommunity.com/app/782330/discussions/0/1867245566135460678/) .

  

  
  



  

