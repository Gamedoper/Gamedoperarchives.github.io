---
layout: post
title:  "How to Setup the Caddy Web Server as a Windows Service"
author: jai
categories: [Technology]
image: assets/img/nssm.png
tags: [featured]
---

# # How to Setup the Caddy Web Server as a Windows Service

### Automatically start Caddy web services whenever your machine boots. 


### Requirements

 1. [Download](https://nssm.cc/download) Nssm 
 2. Add Nssm folder to ENV path Example- path : D:\nssm-2.24\win64
 3. [Download](https://caddyserver.com/v1/download) Caddy Server
 4. Add caddy folder to ENV path 

Env = Environment Variables
After download extract the files in ur Drive.

### Lets make sure its working 

 1. Open Cmd and  type the command Nssm [Test if its working fine]
 
![Caddy file](https://i.imgur.com/Oy4bPPE.png)

 2. Open Cmd and  type the command Caddy [Test if its working fine]

![enter image description here](https://i.imgur.com/GxfHD9A.png)

 
### Add Caddy Server in Nssm 

 - Open Cmd and type Nssm install caddy, Nssm application will be opened
 - Example
 ![nssm_install](https://i.imgur.com/FlXtq5Y.png)
 
 - Now add Caddy.exe path to your nssm 
 ![nssm_caddy](https://i.imgur.com/1KYZnke.png)

Explanation C:

 - Now Im passing Caddy arguments that is -conf [location of caddy conf file]
 - Example : -conf D:\Softwares\CaddyServer\anothercaddyfile.conf
 -  -conf C:\path\to\Caddyfile.conf
- Example of my conf file 
	

        localhost:8888 {
	    root "D:/any folder to be served/"
	    browse
	    gzip
        }


	 The lines following a site address start with a directive. Directives are [keywords that Caddy recognizes](https://caddyserver.com/v1/docs). For example, [gzip](https://caddyserver.com/v1/docs/gzip) is an HTTP directive:

 - For more information about what to add in conf File check the Tutorial of Caddy [Documentation](https://caddyserver.com/v1/tutorial/caddyfile) 

 - Now click on install service .. Caddy service will be successfully.
 - To check the caddy server CLick windows ->start - Services.msc

![services.msc](https://i.imgur.com/pUC2Wp8.png)

 Note : If the services are not running Click on Restart Or Resume in Services msc 
 or
 Open Cmd run this command -> Nssm start caddy(service name you have created) 


## Check your localhost://port files are served

### Hope this article helps, Please post the comment if you face any errors. 
