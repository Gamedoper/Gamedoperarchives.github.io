---
layout: post
title: How to Enable Hyper-V in Windows 10
author: Jai
categories:
  - technology
  - android studio
image: assets/images/powershell_hyperv_twitter.png
tags:
  - summer
---

Virtualization is available to everyone with Windows, and we are going to see how to&nbsp;**enable Hyper-V in Windows 10.**&nbsp;

&nbsp;

## **Enable the Hyper-V role through Settings**

1. Right click on the Windows button and select ‘Apps and Features’.
2. Select&nbsp;**Programs and Features**&nbsp;on the right under related settings.
3. Select&nbsp;**Turn Windows Features on or off**.
4. Select&nbsp;**Hyper-V**&nbsp;and click&nbsp;**OK**.

![](/uploads/settings-2015-05-04-14-21-57.png){: width="415" height="367"}

&nbsp;

## Enable Hyper-V with CMD and DISM

To enable the Hyper-V role using DISM:

1. Open up a PowerShell or CMD session as Administrator.
2. Type the following command:

> DISM /Online /Enable-Feature /All /FeatureName:Microsoft-Hyper-V

PowerShell : One of the quickest ways to start PowerShell, in any modern version of Windows, is to use the Run window. A fast way to launch this window is to press the&nbsp;*Win + R*&nbsp;keys on your keyboard. Then, type&nbsp;*powershell*&nbsp;and press&nbsp;*Enter*&nbsp;or click&nbsp;*OK*.

![](/uploads/dism-upd.png){: width="777" height="348"}

thank you :)