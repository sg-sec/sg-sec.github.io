---
layout: post
title: "Installing RSAT using PowerShell"
tags: [PowerShell, Administration]
date: 2024-04-12
published: true
post_description: A quick guide on installing the Remote Server Administrator Tools (RSAT) using PowerShell.
image: Remote_Administration.jpg
image_alt_text: Large hand controlling puppets
---

Not strictly a security topic but I use the the Remote Server Administrator Tools (RSAT) a lot and its one of the first things I install on a new machine.  This is a quick guide on installing the Remote Server Administrator Tools (RSAT) using PowerShell.

**Table of contents:**
- [List the Installed Tools](#item-two)
- [Install all Tools](#item-three)

<a id="item-two"></a>
#### List the Installed Tools
From a Powershell command prompt run the following command to see if any of the RSAT tools are already installed:

`Get-WindowsCapability -Name RSAT* -Online | Select-Object -Property DisplayName, State`{:.w3-codespan}

<a id="item-three"></a>
#### Install all Tools
From a Administrator Powershell command prompt run the following command to install all of the tools :

`Get-WindowsCapability -Name RSAT* -Online | Add-WindowsCapability -Online`{:.w3-codespan}

If you only want to install a particular tool then change the wild card to be the name of the tool required.
