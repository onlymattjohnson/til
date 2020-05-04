# Change from sh to bash

When installing [Debian](https://www.debian.org/) from scratch on 
[Digital Ocean](https://m.do.co/c/9d2ff49d27e5) the default `ssh` shell is `sh`. 

I want to change this so that I can use autocomplete and other `bash` tools.

For a regular user, change the default login shell using [`chsh`](https://linux.die.net/man/1/chsh):

```bash
chsh -s /bin/bash
```

Alternatively, change the default login shell using `usermod` and replacing _<username>_ 
with the user you want to change this for:

```bash
sudo usermod -s /bin/bash <username>
```
