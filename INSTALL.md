---
layout: default
title: installation guide 
main_nav: false
---

# Installation Guide for Windows

Full details here: http://jekyll.tips/jekyll-casts/install-jekyll-on-windows/

The following is a short summary of what I did to install it. :-)


## Install Chocolately

For detailed description see: See <https://chocolatey.org/install>

### Start command prompt as Administrator

<http://www.howtogeek.com/howto/windows-vista/run-a-command-as-administrator-from-the-windows-vista-run-box/>

* Windows start menu
* Search for cmd
* Press Ctrl-Shift-Enter to start as Administrator

### Install Chocolately

Paste this command to the command prompt

    @powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"


## Install Ruby

Close the cmd.exe command window and open it again (still as Administrator: Search for cmd.exe and press Ctrl-Shift-Enter to run it)

In the Command window use Chocholately to install Ruby

    choco install ruby -y

Install jekyll

    gem install jekyll
    gem install bundler

## Install libraries needed to run the DST4L website

cd to the directory where dst4l is installed

    cd ...<whereever you installed it>....\dst4l

Use bundler to install dst4ls libraries

    bundle install


# Run the website

cd to the directory where dst4l is installed (you are not there already), and then run jekyll :

    jekyll server --watch
