paranoid-prosody
===================

This script is a softer version of paranoid-prosody, and is the version that most normal people might want to use. It has been modified to to enable logging, not force OTR chats, and to not install Tor. If you're not worried about government-level attackers, this is the version for you.

This script bootstraps a Debian/Ubuntu server into being a set-and-forget Prosody server . It's been tested on Debian Wheezy and Ubuntu 14.04, and should work on any other maintained version of those two distros.

not-paranoid-prosody does this:

* Upgrades all the software on the system
* Adds the packages.prosody.im/debian repository to apt, so Prosody updates come directly from the source.
* Installs and configures Prosody with reasonable defaults.
* Configures sane default firewall rules
* Configures automatic updates
* Gives instructions on what the sysadmin needs to manually do at the end

To use it, set up a new Debian or Ubuntu server, SSH into it, switch to the root user, and:

```sh
git clone https://github.com/NSAKEY/not-paranoid-prosody.git
cd not-paranoid-prosody
./bootstrap.sh
```

