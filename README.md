nodejs-deb
==========

**Node + npm package** for linux 64bit made with the latest version by fpm.

###Current verison: 0.10.26

Because package manager is not always up to date and we have to install node AND npm.
So when we are provisioning a server and needed node, it could be a pain to just install node and npm from the command line.

Here you don't have to get worried, we have both in one package.

It's generated with fpm on a precise64 Vagrant virtual machine and the latest source code from http://nodejs.org/dist/node-latest.tar.gz.

Just run ```dpkg -i nodejs-0.10.26_amd64.deb``` and it will do the trick.

I've not tested it on other machine/os, so it may not work on different setup.