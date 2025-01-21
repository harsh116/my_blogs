---
layout: post
title:  "Awesome cli tools"
description: this article list useful and amazing cli tools to make life easier.
tags: awesome cli utilities
---

So i was curious and want to explore some cli tools and i came across this [site](https://dev.to/lissy93/cli-tools-you-cant-live-without-57f6). So i discovered some nice tools which i noticed and wanna share them and what i think about them


### Contents
---
1. [zoxide](#zoxide)
2. [eza and lsd](#eza-and-lsd)
3. [bat](#bat)
4. [duf](#duf)
5. [fzf](#fzf)
6. [hyperfine](#hyperfine)
7. [jq](#jq)
8. [dua-cli](#dua-cli)
9. [bandwhich](#bandwhich)
10. [ddgr and googler](#ddgr-and-googler)
11. [micro](#micro)
12. [lazydocker](#lazydocker)
13. [lazygit](#lazygit)
14. [mycli](#mycli)
15. [tldr](#tldr)
16. [yazi](#yazi)
17. [asciinema](#asciinema)
18. [toilet and figlet](#toilet-and-figlet)
19. [cowsay](#cowsay)

---



### zoxide
zoxide is a smarter cd command, inspired by z and autojump. cd itself is fine but when we open terminal we don't wanna type whole directory every time so this tool is quite useful.

**Usage**
```bash
> z ~/Downloads/Compressed
> z ..
> z Compressed
```

**Source code**

<https://github.com/ajeetdsouza/zoxide>{:target="_blank"}

&nbsp;
### eza and lsd
eza is a modern alternative for the venerable file-listing command-line program ls. Similarly there is `lsd`. Both are written in Rust and there are few differences in syntax too.

**Usage**
```bash
# for listing treeview of contents of current directory with max depth 2

# with eza
eza --oneline --icons --tree -L 2

# with lsd
lsd --tree --depth 2
```

**Source code**

<https://github.com/eza-community/eza>{:target="_blank"} and <https://github.com/lsd-rs/lsd>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/eza demo.png)


&nbsp;
### bat
A cat(1) clone with wings. It is cat that comes with syntax highlighting and automatic paging. Very useful to get a quick look of contents of file with syntax highlighting

**Usage**
```bash
> bat file.txt
```

**Source code**

<https://github.com/sharkdp/bat>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/bat demo.png)

&nbsp;
### duf
It stands for Disk Usage/Free Utility and is  a better 'df' alternative which can give a user friendly colorful output. Just type `duf`

**Source code**

<https://github.com/muesli/duf>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/duf demo.png)

&nbsp;
### fzf
**Highly recommended**

A command-line fuzzy finder. It is interactive filter which indexes list and can show the result instantly.

**Usage**
```bash
find * -type f | fzf > selected
```

**Source code**

<https://github.com/junegunn/fzf>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/fzf demo.png)

&nbsp;
### hyperfine
A command-line benchmarking tool. Supports features like statistical analysis,constant feedback,warmup,etc. Good for those who wanna check and compare speed of different commands.

**Usage**
```bash
hyperfine  "find /mnt/hdd/Movies -type f"
```

**Source code**

<https://github.com/sharkdp/hyperfine>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/hyperfine demo.png)

&nbsp;
### jq
jq is a lightweight and flexible command-line JSON processor. One of its useful feature that i have found is printing pretty and colorful output of json file.

**Usage**
```bash
jq . package.json
```

**Source code**

<https://github.com/jqlang/jq>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/jq demo.png)

&nbsp;
### dua-cli
View disk space usage and delete unwanted data, fast. Sometimes we wanna see disk usage of files and folders in directories. It is true that `ls -l` exists but it dont show
size information of directories itself so this is very helpful and have its interactive version too.

**Usage**
```bash
# normal version
dua

# interactive version
dua interactive
```

**Source code**

<https://github.com/Byron/dua-cli>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/dua-cli demo.png)
![](/assets/images/posts/2024-02-24-awesome-cli-tools/dua-cli interactive demo.png)

&nbsp;
### bandwhich
**Highly recommended**

This is a CLI utility for displaying current network utilization by process, connection and remote IP/hostname. Very useful to monitor which software or process is utilizing network and how much. I needed this tool which does that and keeps me informed which process is using internet connection.

**Source code**

<https://github.com/imsnif/bandwhich>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/bandwhich demo.png)

&nbsp;
### ddgr and googler
It is always helpful to get quick search result without opening browser and type it so this can be useful

**Usage**
```bash
ddgr internet
```

**Source code**

<https://github.com/jarun/ddgr>{:target="_blank"} and <https://github.com/jarun/googler>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/ddgr demo.png)

&nbsp;
### micro
**Highly recommended**

This is a TUI editor which is easy to use and simple. It supports syntax highlighting for many languages. You maybe thinking that why use this when we have nano, vim, emacs, etc.
It is true that those editors are awesome in their own way but for many users who are not used to their specific keybindings can use this as comes with common keybindings
which makes editing in it way more productive for those who are used to GUI text based editor.

Also some people says 'Why not use GUI text editors?' Answer is simple, when connecting to servers they dont have GUI for most cases so a editor which dont have any steep learniing curve and is easy to use is quite handy.

**Source code**

<https://github.com/zyedidia/micro>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/micro demo.png)

&nbsp;
### lazydocker
TUI interface for managing docker containers,images and volumes and to keep tracks and monitor too. It is true that commands exists but sometimes it can be frustrating to use those commands everytime and we want some convinient way so thats where this tool comes.

**Source code**

<https://github.com/jesseduffield/lazydocker>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/lazygit demo.png)

&nbsp;
### lazygit
**Highly recommended**

TUI interface to manage git repository, just like lazydocker and made by same developer and written in Go too. Very useful and highly recommend it to check this out.

**Source code**

<https://github.com/jesseduffield/lazygit>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/lazydocker demo.png)

&nbsp;
### mycli
mysql is cool dbms and have its shell too. mysql workbench is used to get features like syntax highlighting and auto-complete. So why not have something in shell instead. This is where this tool comes in.
It is a terminal client for MySQL with autoCompletion and syntax highlighting.

**Source code**

<https://github.com/dbcli/mycli>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/mycli demo.png)

&nbsp;
### tldr
**Highly recommended**

This is a collaborative cheatsheets for console commands. man pages and `--help` exists but they are too comprehensive and sometimes users need to know some main commands rather than read whole manual just to test it.
Thats where tldr comes in, It contains community-maintained list of some main commands. tldr is not a full replacement of man because user may wanna know more commands but tldr covers main commands so it is very useful and saves times of surfing them in browser.

**Usage**
```bash
tldr grep
```

**Source code**

<https://github.com/tldr-pages/tldr>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/tldr vs man.png)

&nbsp;
### yazi
Blazing fast terminal file manager written in Rust, based on async I/O. yazi file manager. This file manager is wonderful in sense that it can peek through files and folders and displays contents inside zip files, text files and also thumbnail for images,videos,etc and
can be configured to open with whatever program user wants. Very useful to surf through and all in terminal means it can be used for servers too which don't have GUI.

**Source code**

<https://github.com/sxyazi/yazi>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/yazi demo.png)

&nbsp;
### asciinema
**Highly recommended**

It is a terminal session recorder.
This is such a unique thing i have seen and was surprised. what it does it to make a recording of terminal and when someone plays this recording , he can interact with its text too. So a great tool  to make tutorials and all that.

**Source code**

<https://github.com/asciinema/asciinema>{:target="_blank"}

[![asciicast](https://asciinema.org/a/85R4jTtjKVRIYXTcKCNq0vzYH.svg)](https://asciinema.org/a/85R4jTtjKVRIYXTcKCNq0vzYH)

&nbsp;
### toilet and figlet
So till now I have talked about some useful utilities but some times its good to have something interesting and fun so lets talk about them too.
FIGlet is a program that creates large characters out of ordinary screen characters.
Similarly there is toilet which is inspired my figlet that comes with more art.

**Usage**
```bash
toilet hello --filter metal
```

**Source code**

<https://github.com/cacalabs/toilet>{:target="_blank"} and  <https://github.com/cmatsuoka/figlet>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/toilet demo.png)
![](/assets/images/posts/2024-02-24-awesome-cli-tools/figlet demo.png)

&nbsp;
### cowsay
cowsay is a program that generates ASCII art pictures of a cow with a message. It can also generate pictures using pre-made images of other animals, such as Tux the Penguin, the Linux mascot. It is written in Perl.
It can be used to send them in social media or use it anywhere where images are not allowed or feasible. Like figlet/toilet, they are need to be monospace font

**Usage**
```bash
# eyes here is art and hello is the text
cowsay -f eyes hello
```

**Source code**

<https://github.com/cowsay-org/cowsay>{:target="_blank"}

![](/assets/images/posts/2024-02-24-awesome-cli-tools/cowsay demo.png)
