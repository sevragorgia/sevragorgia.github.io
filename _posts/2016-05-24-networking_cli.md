---
layout: post
section-type: post
title: Title
category: Linux 
tags: [ 'Linux', 'CLI tricks' ]
---

I use ubunut and just deleted my windows system... I removed (with --purge and all) gdm. So, today, when I started my laptop I only got a black screen... no window manager, nothing.

I was in my office, where I cannot plug my laptop to the wired network and needed to connect to a specific wlan that requires a profile to authenticate my user. Within gnome or unity this is just a click, but without them...

Anyway, I found the trick after 0s googling. You can interact with the NetworkManager using the commands *nmcli*.

*nmcli con* will list all NM available connections.

*nmcli con up id ConnectionName* will connect to the desired network.

using this commands I could connect to the wlan and reinstall gnome... Now I am blogging about this. If I had called the technical support or an IT company to "repair" my laptop it would have cost me alot of money... and there was nothing to repair...

Thanks to:

http://askubuntu.com/questions/57339/connect-disconnect-from-vpn-from-the-command-line





