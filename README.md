 ssh-mpv
===========

List and play videos over ssh using [mpv](https://mpv.io/).

 Dependencies
----------------

Dependencies needed for the script to work properly.

- [mpv](http://mpv.io/): mplayer fork with enhancements
- [SSH](https://de.wikipedia.org/wiki/Secure_Shell): Secure Shell to get access on your remote video files
- [fzf](https://github.com/junegunn/fzf): command-line fuzzy finder

Install it on linux:
```bash
sudo apt update
sudo apt install openssh mpv fzf
```

 Variables
-------------

Edit the following variables in the script before use.

- user: ssh server user
- server: ssh server name 
- port : port to use for ssh (22 by default)
- dir: directory to search on the ssh server

*And you have the option to use a [Jump Host](https://www.tecmint.com/access-linux-server-using-a-jump-host/) to access the server indirectly if he is e.g. behind a NAT/Firewall)*

## Usage

```bash
    ssh-mpv [opt] <search...>
```

### Options
```bash
- h: list the help page
- l: list remote videos to stdout
```

## Add SSH Key
```bash
ssh-copy-id -i ~/.ssh/key user@host
```
