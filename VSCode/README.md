# [  VS Code ]

## Install VS Code

*From: https://code.visualstudio.com/*

Download the Linux x64 .deb file at `https://code.visualstudio.com/` website

Move the .deb file to the `~/smartcampusmaua/smartcampusmaua-tools/VSCode/src` directory
```bash
mkdir -p ~/smartcampusmaua/smartcampusmaua-tools/VSCode/src
mv ~/Downloads/code*.deb ~/smartcampusmaua/smartcampusmaua-tools/VSCode/src
```

Install the code*.deb file at the ~/Tools/VSCode/src directory
```bash
cd ~/smartcampusmaua/smartcampusmaua-tools/VSCode/src
sudo dpkg -i code*.deb
```

Validate the installation just verifying if node and npm commands are avaiable from the Terminal

```bash
code -v
----
1.66.2
dfd34e8260c270da74b5c2d86d61aee4b6d56977
x64
----
```

Thats it! The system is ready to use VSCode!

