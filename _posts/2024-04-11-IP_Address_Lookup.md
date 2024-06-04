---
layout: post
title: "Using the command line to get IP address information"
tags: OSINT
date: 2024-04-11
published: true
post_description: I often need to look up IP addresses to find out useful information.  This is how I do it from the command line.
image: IP_address_search.jpg
image_alt_text: Magnifying glass zooming in on scrolling IP addresses
---
I often need to look up IP addresses to find out useful information such as the geo-location.  This is how I do it from the command line.


**Table of contents:**
- [Command Line Example](#item-two)
- [More Information and Examples](#item-three)

<a id="item-two"></a>
#### Command Line Example
From a command prompt (either CMD or Powershell) run the following command:

`curl.exe ipinfo.io/8.8.8.8`{:.w3-code}

<a id="item-three"></a>
#### More Information and Examples
You'll notice that I used curl.exe rather than curl.  This is because Powershell comes with a curl alias which I don't like.  The curl.exe is far more powerful and I prefer the output format.

If you want to get your internet facing IP address try this command:

`curl.exe ipinfo.io/IP`{:.w3-code}

If you get certificate errors whilst running the curl command you can use the -k command argument to override the error:

`curl.exe -k ipinfo.io/8.8.8.8`{:.w3-code}

Use the -v command argument for verbose output:

`curl.exe -v ipinfo.io/8.8.8.8`{:.w3-code}

Hope this has been useful.
