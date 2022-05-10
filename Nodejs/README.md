# [ Install Nodejs, npm and yarn ]

## Install Nodejs and npm

*From: https://nodejs.org/en/download/*

Download the Linux x64 binarries at https://nodejs.org/en/download/ website

Move the node-v16.15.0-linux-x64.tar.xz file to the ~/Tools/Nodejs directory
```bash
mkdir -p ~/smartcampusmaua/smartcampusmaua-tools/Nodejs/src
mv ~/Downloads/node-v16.15.0-linux-x64.tar.xz ~/smartcampusmaua/smartcampusmaua-tools/Nodejs/src
```

Uncrompress the node-v16.15.0-linux-x64.tar.xz file at the ~/Tools/Nodejs directory
```bash
cd ~/smartcampusmaua/smartcampusmaua-tools/Nodejs/src
tar -vxf node-v16.15.0-linux-x64.tar.xz -C ../
```
Open the `~/.bashrc` or `~/.zshrc` file and include the Nodejs binaries in the environment variable called PATH in the last lines of this file configure the Linux Terminal default options.
```bash
nano ~/.bashrc
# or 
nano ~/.zshrc
```

Then, add in the last line of the file:
```bash
# Set Nodejs to the PATH
export PATH=$PATH:~/smartcampusmaua/smartcampusmaua-tools/Nodejs/node-v16.15.0-linux-x64/bin
```

Save and Exit the file editor with Ctrl^O, ENTER, Ctrl^X

If the Terminal is open, the Terminal`s configuration file must be reload.
```bash
source ~/.bashrc
# or
source ~/.zshrc
```

Or just close the Terminal with Ctrl^D or exit command or just closing then reopening, the changes shall be applied too.


Validate the installation just verifying if node and npm commands are avaiable from the Terminal

```bash
node -v
----
v16.15.0
----
```

```bash
npm -v
----
8.5.5
----
```


## Install Yarn with npm

*From: https://classic.yarnpkg.com/en/docs/install/#debian-stable*

There is a recommendation to install Yarn through the npm package manager, which comes bundled with Node.js when is is install it on the system.

Once npm is installed, please run the following both to install and upgrade Yarn:

```bash
npm install --global yarn
```

Check the installation by running

```bash
yarn -v
----
1.22.18
----
```


Thats it! The system is ready to use node, npm and yarn commands!
