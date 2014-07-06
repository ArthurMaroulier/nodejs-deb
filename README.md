nodejs-deb
==========

**Node + npm package** for linux 64bit made with the latest version by fpm.

###Current version of node: 0.10.29

Because package manager is not always up to date and we have to install node AND npm.
So when we are provisioning a server and needed node, it could be a pain to just install node and npm from the command line.

Here you don't have to get worried, we have both in one package.

It's generated with fpm on a precise64 Vagrant virtual machine and the latest source code from http://nodejs.org/dist/node-latest.tar.gz.

Just run ```dpkg -i nodejs-0.10.29_amd64.deb``` and it will do the trick.

####For provisioning use
There's also a version that comes with a generic file name ```nodejs_amd64.deb```.

So you can use the raw link in your provisioning scripts: ```https://github.com/ArthurMaroulier/nodejs-deb/raw/master/nodejs_amd64.deb```


####Warning
I've not tested it on other machine/os, so it may not work on different setup.



For Raspberry pi
----------------
###Current version of node: 0.10.25

Just download the latest version of ```linux-arm-pi``` tar.gz file from nodejs.com :

```wget http://nodejs.org/dist/v0.10.25/node-v0.10.25-linux-arm-pi.tar.gz```

Run ```tar -xvzf node-v0.10.25-linux-arm-pi.tar.gz``` to the directory of your choice.

Set the ```NODE_JS_HOME``` variable to this directory and add the bin dir to your ```PATH```:

```
NODE_JS_HOME=/path/to/node-v0.10.25-linux-arm-pi 
PATH=$PATH:$NODE_JS_HOME/bin 
```
Now you can run node and npm from anywhere.

```node --version``` should return v0.10.25.

```npm -version```should return 1.3.24.


If you need you can install node's native build tool ```node-gyp``` :

```npm install -g node-gyp```
