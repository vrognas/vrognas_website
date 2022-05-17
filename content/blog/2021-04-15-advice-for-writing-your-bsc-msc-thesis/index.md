---
title: "Cheat the command line"
subtitle: ""
date: "2020-06-08"
author: "Viktor Rognås"
draft: true
# layout options: single, single-sidebar
layout: single
categories:
- cli
---

When you start out using the command line, you will notice that there are many small and handy programs (also referred to as *commands*) you can run. You might start out using `pwd` (for *print working directory*), which will tell you what directory you are currently in. Then you might use programs such as ls to *list* the contents of a directory, and you might use `cd` to *change directory* to another directory you might want to go to.

Well there are obviously many many more programs like this, and to know more about them the most important command to know about is the command man (for *manual*). If you run e.g. `man pwd`, you will get to the manual page for the `pwd` command which will tell you most things there are to know about the `pwd` command.

Now, this particular man page is not that lengthy, but what if you run `man ls`, or what about `man ffmpeg` (`ffmpeg` deals with multimedia conversion)? Now that’s quite some documentation to go through!

A quicker way to just get the gist of a command can be accessed via https://cheat.sh (it is a web site on it's own, go check it out). You can also access cheat.sh on the command line via curl cheat.sh (or even `curl cht.sh`!). To get the gist of a command, just type: `curl cht.sh/ls`, and you will get the gist of the ls command! Replace ls with any command you like.

Another way I prefer is to use the `tldr` command, which in essence is the same as cheat.sh in that it is a community-driven manual. However, I have found that `tldr` gives a bit more relevant information for macOS which is the operating system I am using as my daily driver. The `tldr` program does not come pre-installed but you can find the installation information here: https://tldr.sh

If you are on macOS you can install it with `brew install tldr`.

To use `tldr`, just type `tldr ls` in your terminal, replace `ls` with the command you would like to know about.
