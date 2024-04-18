---
layout: post
title: "Password Protecting SSH Keys (PEM files)"
tags: SSH
date: 2024-04-18
published: false
image: Secure_SSH.jpg
image_alt_text: A pad lock sitting on a sheild with a golden auroa
---
<!-- Description of article -->
Although not ideal from time to time it is required to store SSH keys (PEM files) locally on your machine.  If you do this you should password protect those files.  

**Table of contents:**
- [Password Protecting the SSH Key](#item-one)
- [Using the Key](#item-two)

<!-- headings -->
<a id="item-one"></a>
#### Password Protecting the SSH Key
This process presumes that your keys are stored under c:\users\<username>\.ssh

From the command line run the following command:

ssh-keygen -p -f .ssh/name_of_file

You will then be asked to enter passphrase.  Enter a strong passphrase and store it in your password vault.

Now when you use the key you will be asked to provide a passphrase for the key.

<a id="item-two"></a>
#### Using the Key
Example:

ssh -i .\Example_Key.pem user_name@server_name

