---
title: How to set up SSH to connect on a different port (or a different key)
author: jaidev
categories:
  - jd
tags:
  - linux
published: true
---
I was looking for a way to connect via SSH to a git server, on a different port (other than 22), and using a different identity file ([see below](#Different-SSH-identity-files)).

It turns out that the easiest way to do this is by setting up an ssh config file (see `man ssh_config`), at `~/.ssh/config`. Following the directions [here, by C. Pino](https://web.archive.org/web/20191219052807/https://medium.com/@czarpino/how-to-tell-git-which-ssh-key-to-use-c8574fb243fd), I included in the the ssh config file:

```
# ~/.ssh/config
Host my.hostname.com
    Hostname hostname.com
    User git
    IdentityFile ~/.ssh/key_to_use
```

If you see the error: `Bad owner or permissions on /home/jd/.ssh/config`, ensure the config file has `rw` only access for the user (hint from the [serverfault.com post here](https://serverfault.com/questions/253313/ssh-returns-bad-owner-or-permissions-on-ssh-config)):

```
$ chown $USER ~/.ssh/config
$ chmod 600 ~/.ssh/config
```

## Different SSH identity files

I decided to go ahead and create different key pairs for each of the online services I use. Using the Github documentation ([here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)), the method I used for each key was:

```
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
> Generating public/private rsa key pair.

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

> Enter a file in which to save the key (/home/you/.ssh/id_rsa): [enter filename 1 for first keypair]

At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".

> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]
```

I added the keypair to the ssh-agent, and made sure that the correct keys are referenced in the ssh_config file:

```
$ eval "$(ssh-agent -s)"
> Agent pid 59566
ssh-add ~/.ssh/filename1
```

I am now able to connect to my ssh server (using git) via: 

`git clone git@your.hostname.com:path/to/gitfile.git`.




