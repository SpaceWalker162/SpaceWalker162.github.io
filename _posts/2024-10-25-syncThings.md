---
title: Sync Between My Laptop and Desktop
date: 2024-10-25
permalink: /posts/2024/joifwjhfwiwfd
excerpt_separator: <!--more-->
toc: true
tags:
  - web-dev
---
Some notes on remote access.
<!--more-->

## Introduction
Since I am working with an increasing number of computers, it is increasingly
important to efficiently transfer/sync files and applications/programs across
this network of computers.

Previously I used my laptop as the major computer for daily work, including
searching, reading, researching, writing and so on. Heavy computational work
is assigned to several desktops in my lab. A large database is attached to the
local network in the lab to facilitate fast access and analysis of data.
Occasionally, I also do some light data analysis on my laptop.

In this scenario, common programs such as `python` (anaconda with some
additional modules), `vim` and `tmux` are installed on these computers. SSH is used
for remote control and occasional transfer of files. `git` is used for syncing
scripts. `rsync` is used to transfer large amount of files.

Recently I have bought a new desktop for my home so I have a large screen
to view images (why not TV screen?). Therefore, I prefer the
desktop over the laptop at home. However, when not at home I need to use the laptop. Here comes a need for syncing between these two computers. The ideal solution is very simple, thanks to them both being with MacOS, which is to use `icloud` synchronization. Yet given the limited funding and the readily available large storage in the lab, I am using [syncthing](https://syncthing.net) to make the storage in lab a cloud storage node/server and syncing from it to my laptop and desktop at home.
