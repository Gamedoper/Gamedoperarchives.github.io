---
layout: post
title: 'Batman: Arkham Knight''s framerate stutters with DX11 hooking'
author: Gamedoper
categories:
  - GAMEERRORFIX
image: assets/images/batman.jpg
tags:
  - sticky
---

# Batman: Arkham Knight's framerate stutters Fix.

![enter image description here](https://i.imgur.com/nTUmCRb.png)

Batman: Arkham Knight is one of PC game, suffering from stuttering and Glitching issues which make the game challenging to play on even today's highest-end hardware.

Batman fans rejoice, because we may finally have a fix for Batman's frame rate woes, all thanks to the PC modder SheriefFarouk, who has created a mod which is designed to stabilise Arkham Knight's frame rates on PC.

After an in-depth performance investigation of the game, SheriefFarouk uncovered a potential cause of Arkham Knight's frame rate issues. The simple way of describing the problem is that Arkham Knight doesn't handle texture generation correctly, creating thousands of new textures on the fly, rather than reusing and recycling them whenever possible. Using his fix, Sharief has managed to stabilise Arkham Knight's frame rates on PC, albeit with some compatibility issues.

SheriefFarouk has seemingly fixed this issue with a simple DLL file.

**Installation**

The installation of Arkham Knight's PC fix is simple. **Add the drop-in D3D11 DLL** file into the same directory as your BatmanAK.exe file and you are ready to go. This file can be downloaded on [**Sherief's website**](https://sherief.fyi/post/arkham-quixote/) and the source code of the fix is available on [**GitHub**](https://code.sherief.fyi/sherief/arkham-fixer/src/branch/batman).

[Download DLL](https://sherief.fyi/arkham-knight/dxgi.dll)