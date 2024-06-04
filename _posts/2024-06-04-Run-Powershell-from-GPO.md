---
layout: post
title: "Run Powershell from a GPO"
tags: Powershell GPO
date: 2024-06-04
published: true
image: Powershell_from_GPO.jpg
image_alt_text: Powerful super hero with Powershell command prompts
---
<!-- Description of article -->
Getting a Powershell script to run from a GPO should be easy.  You should be able create a GPO, go to Computer Configuration > Policies > Windows Settings > Scripts > Startup (or Shutdown) and enter the path to your script on the PowerShell Script tab.  
For some reason I have found that this doesn’t work every time.

I find the following configuration to be more reliable.

#### Example Configuration

