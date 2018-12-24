---
layout: post
title: Linux notes
categories: [it]
tags: [Linux]
---

## PackageManage
1. List the installed software packages on Ubuntu
<div class="terminal" markdown="1">
`$ sudo apt list --installed`
</div>
2. Completely remove intalled software includes configuration
<div class="terminal" markdown="1">
`$ sudo apt purge <package-name>`
</div>
3. [apt vs apt-get difference](https://itsfoss.com/apt-vs-apt-get-difference)
4. Debian operating system ==> dpkg packaging system: from high to low 
  - `apt`, most used command in `apt-get` and `apt-cache`
  - `apt-get` && `apt-cache` etc. upgrade, search, install dependenies and more
  - `dpkg`, install && remove && build(dpkg-deb)
  - `dpkg-deb`, build && manipulate archive(.deb)
5. APT: Advaced Package Tool || apt: high-level command line interface
