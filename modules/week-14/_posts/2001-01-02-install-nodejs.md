---
title: Install node.js
module: 14
jotted: true
---

# Install node.js

There is an option to try node.js without installing it. It's located here.

<a href="https://www.tutorialspoint.com/execute_nodejs_online.php" target="_new">Online node.js</a>

Local Environment Setup
If you are still willing to set up your environment for Node.js, you need the following two softwares available on your computer, (a) Text Editor and (b) The Node.js binary installables.

Text Editor
This will be used to type your program. Examples of few editors include Windows Notepad, OS Edit command, Brief, Epsilon, EMACS, and vim or vi.

Name and version of text editor can vary on different operating systems. For example, VS Code or Atom will work just fine.

The files you create with your editor are called source files and contain program source code. The source files for Node.js programs are typically named with the extension ".js".

Before starting your programming, make sure you have one text editor in place and you have enough experience to write a computer program, save it in a file, and finally execute it.

The Node.js Runtime

The source code written in source file is simply javascript. The Node.js interpreter will be used to interpret and execute your javascript code.

Node.js distribution comes as a binary installable for SunOS , Linux, Mac OS X, and Windows operating systems with the 32-bit (386) and 64-bit (amd64) x86 processor architectures.

Following section guides you on how to install Node.js binary distribution on various OS.

Download Node.js archive
Download latest version of Node.js installable archive file from Node.js <a href="https://nodejs.org/download/" target="_new">Downloads</a>. At the time of writing this tutorial, following are the versions available on different OS.

OS	Archive name

Windows	node-v6.3.1-x64.msi
Linux	node-v6.3.1-linux-x86.tar.gz
Mac	node-v6.3.1-darwin-x86.tar.gz
SunOS	node-v6.3.1-sunos-x86.tar.gz

Installation on UNIX/Linux/Mac OS X, and SunOS
Based on your OS architecture, download and extract the archive node-v6.3.1-osname.tar.gz into /tmp, and then finally move extracted files into /usr/local/nodejs directory. For example:

$ cd /tmp
$ wget http://nodejs.org/dist/v6.3.1/node-v6.3.1-linux-x64.tar.gz
$ tar xvfz node-v6.3.1-linux-x64.tar.gz
$ mkdir -p /usr/local/nodejs
$ mv node-v6.3.1-linux-x64/* /usr/local/nodejs
Add /usr/local/nodejs/bin to the PATH environment variable.

OS	Output

Linux	export PATH=$PATH:/usr/local/nodejs/bin
Mac	export PATH=$PATH:/usr/local/nodejs/bin
FreeBSD	export PATH=$PATH:/usr/local/nodejs/bin
Installation on Windows
Use the MSI file and follow the prompts to install the Node.js. By default, the installer uses the Node.js distribution in C:\Program Files\nodejs. The installer should set the C:\Program Files\nodejs\bin directory in window's PATH environment variable. Restart any open command prompts for the change to take effect.

Verify installation: Executing a File

Create a js file named main.js on your machine (Windows or Linux) having the following code.

```js
/* Hello, World! program in node.js */
console.log("Hello, World!")
```

Now execute main.js file using Node.js interpreter to see the result −

```js
$ node main.js
```
If everything is fine with your installation, this should produce the following result −

`Hello, World!`
