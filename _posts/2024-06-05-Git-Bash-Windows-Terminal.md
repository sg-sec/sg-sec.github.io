---
layout: post
title: "Adding a Git Bash profile to Windows Terminal"
tags: Git
date: 2024-06-05
published: true
image: generic_Terminal_Coding.jpg
image_alt_text: Image of a terminal with code
---
<!-- Description of article -->
A quick guide on how to configure a Git Bash profile in Windows Terminal


<div class="w3-panel w3-light-blue"><p><span class="w3-badge w3-indigo">i</span> This guide presumes that Git is installed under the users profile location and that your working Git folder is c:\git.  You might need to adjust the guide accordingly.</p></div>

#### Configuration
1. Open the Windows Terminal
2. Open the Settings page. Pressing "ctrl" + "," will do this for you.  
3. Select the ***Add New Profile*** button.
4. Click on the ***New Empty Profile*** button.
5. Set the ***Name*** field to ***Git Bash***
6. Set the ***Command Line field*** to be:
   
   `C:\Users\<username>\AppData\Local\Programs\Git\bin\bash.exe`{:.w3-code}
   
7. Set the ***Starting Directory*** to be:
   
   `C:\git`{:.w3-code}
   
8. Click on Save.
