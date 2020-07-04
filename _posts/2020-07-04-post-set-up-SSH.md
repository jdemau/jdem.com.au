---
title: How to set up SSH to connect on a different port (or a different key)
author: jaidev
categories:
  - jd
tags:
  - linux
---
## How to set up SSH to connect on a different port (or a different key)

I was looking for a way to connect via SSH to a git server, on a different port (other than 22), and using a different identity file (see below).

It turns out that the easiest way to do this is by setting up an ssh config file (see `man ssh_config`), at `~/.ssh/config`. Following the directions [here, by C. Pino](https://web.archive.org/web/20191219052807/https://medium.com/@czarpino/how-to-tell-git-which-ssh-key-to-use-c8574fb243fd), the ssh_config file should include:

```
# ~/.ssh/config
Host your.hostname.com
    Hostname hostname.com
    User git
    IdentityFile ~/.ssh/key_to_use
```

If you see the error: `Bad owner or permissions on /home/jd/.ssh/config`, ensure you have rw only access for the user (from the [serverfault.com post here](https://serverfault.com/questions/253313/ssh-returns-bad-owner-or-permissions-on-ssh-config)):

```
# chown $USER ~/.ssh/config
# chmod 600 ~/.ssh/config
```
