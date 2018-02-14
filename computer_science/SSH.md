# SSH
| Useful Links     |                                                    |
|------------------|----------------------------------------------------|
| Arch Wiki        | https://wiki.archlinux.org/index.php/Secure_Shell  |
| LUG Presentation | https://github.com/sumnerevans/lug-ssh             |

## Overview

**S**ecure **Sh**ell (SSH) is a way to login and execute commands on remote
servers. For example, you can SSH to `isgengard`, a really nice server
accessible to all Mines students, and run commands on it as if you were at the
physical server.

## Installing SSH

### Linux

SSH is in your distribution's package manger, and likely already installed.

- **Arch:** `openssh`
- **Ubuntu:** `openssh-client`
- **Fedora:** `openssh-client`

### macOS

Install the
[`openssh`](http://formulae.brew.sh/repos/Homebrew/homebrew-core/formula/openssh)
formula using [Homebrew](./Homebrew.md).

### Windows

TODO: this documentation is incomplete. Someone who actually uses Windows should
update this.

You can use PuTTY.

You can also use the Linux Subsystem if you have Windows 10.

## Using SSH

SSH can be used to log in to remote servers.

### Logging in to Remote Servers

To login to a server, type:

    ssh [<username>@]<server>

where `<server>` is the server you want to log in to, and `<username>` is the
user to log in as. Everything inside the brackets (`[]`, inclusive) is optional.
If `<username>` is not specified, it will default to your current machine's
username.

## Creating an SSH Key

Creating an SSH key will allow you to log into remote servers without entering
your password every single time.

IN PROGRESS

### Using SSH With Git

IN PROGRESS

## Configuring SSH

You can add entries to your `~/.ssh/config` file (create it if it doesn't
exist). Entries take the form:

    Host <hostname>
        <Property> <value>
        ...

You can also add global properties that are set on all servers using:

    <Property> <value>

**Example `~/.ssh/config` file:**

    # Defaults
    IdentityFile ~/.ssh/id_rsa

    Host arrakis
        HostName arrakis.mines.edu
        Port 8080
        User foo

Now, you can type `ssh arrakis` and SSH will attempt open a connection to
`arrakis.mines.edu` on port `8080` and authenticate as user `foo` with the
identity file located at `~/.ssh/id_rsa`.
