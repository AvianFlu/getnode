# getnode - install Node.JS from source, no thinking required!

When you're not used to it, the idea of compiling something from source can be
scary.  It's not very difficult once you're used to it, but that distribution's
package manager... it just seems so much easier... and it's not that bad to be a
few versions behind, is it?

Well, with Node.JS, being a few versions behind isn't a great idea.  You're
missing out on important improvements and bug fixes to a fairly young,
still-stabilizing platform.  

## Stop waiting for the package manager to update - getnode!

### Installation

     git clone https://github.com/AvianFlu/getnode

### Usage

     cd getnode
     ./getnode 0.6.10

The version of node specified will be downloaded, decompressed, compiled, and
installed while you wait.

### I got an error after compiling!

Node tries to put itself in `/usr/local/bin` by default.  Because `getnode`
includes a call to `curl`, it does not attempt to run itself as root.  Try `sudo make
install` after `getnode` exits.
