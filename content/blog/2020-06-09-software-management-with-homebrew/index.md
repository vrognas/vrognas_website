---
title: "Software management on macOS with Homebrew \U0001F37A"
subtitle: ""
author: Viktor Rognås
date: "2020-06-09"
categories:
  - cli
  - macOS
  - Geeky stuff
draft: false
# layout options: single, single-sidebar
layout: single
---

One thing that GNU/Linux users are familiar with is the concept of a “package manager”.
A package manager is a tool that keeps track of software for you.
It installs it, uninstalls it, upgrades it, etc.
On macOS there isn’t any package manager installed by default 
(perhaps the App Store could be seen as some form of package manager?), 
so for all you macOS users out there I highly recommend you install [Homebrew](https://brew.sh/).

All you have to do is literally paste this into your terminal, and then follow the instructions:
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`

## Install/upgrade software on a remote server without admin rights

The above script also works on remote Linux servers.
If you run this script, then you will get a folder “.linuxbrew” in your home 
user folder which will contain all your programs. 
This is nice to have if your server runs old software e.g. old git versions 
(I’m looking at you, CentOS!).

## Using Homebrew 🍺

On the command line, type e.g. `brew search firefox` to search for “firefox”, 
you can search for any software you like. 
For command line utilities (“formulas”), these are installed with 
`brew install wget` (to install the formula `wget`), for proper software 
applications (“casks”) like Firefox, these are installed with `brew cask install firefox`.
I recommend installing all your software with Homebrew since it is much easier 
to keep track of programs och your system this way, and a nice feature is that 
you can upgrade all programs in one sweep by just typing `brew upgrade` and hit 
Enter in your terminal.

To list all installed formulas, just type `brew list`, and for casks type `brew cask list`.
