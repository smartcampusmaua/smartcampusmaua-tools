# [  Open Java SE Development Kit 11 ]

## Install Open JDK 11

*From: https://jdk.java.net/java-se-ri/11*

Download the Linux x64 `.tar.gz` binarries at https://jdk.java.net/java-se-ri/11 website

Move the tar.gz file to the ~/Tools/Java/OpenJDK directory
```bash
mkdir -p ~/smartcampusmaua/smartcampusmaua-tools/Java/OpenJDK/src
mv ~/Downloads/openjdk-11+28_linux-x64_bin.tar.gz ~/smartcampusmaua/smartcampusmaua-tools/Java/OpenJDK/src
```

Uncrompress the `openjdk-11+28_linux-x64_bin.tar.gz` file at the `~/smartcampusmaua/smartcampusmaua-tools/Java/OpenJDK/src` to a directory before.
```bash
cd ~/smartcampusmaua/smartcampusmaua-tools/Java/OpenJDK/src
tar -vxf openjdk-11+28_linux-x64_bin.tar.gz -C ../
```

Open the `~/.bashrc` or `~/.zshrc` file and include the Jav OpenJDK binaries in the environment variable called PATH in the last lines of this file configure the Linux Terminal default options.
```bash
nano ~/.bashrc
# or 
nano ~/.zshrc
```

Then, add in the last line of the file:
```bash
# Set Java OpenJDK binaries to the PATH
export PATH=$PATH:~/smartcampusmaua/smartcampusmaua-tools/Java/OpenJDK/jdk-11/bin
```

Save and Exit the file editor with Ctrl^O, ENTER, Ctrl^X

If the Terminal is open, the Terminal`s configuration file must be reload.
```bash
source ~/.bashrc
# or
source ~/.zshrc
```

Or just close the Terminal with Ctrl^D or exit command or just closing then reopening, the changes shall be applied too.


Validate the installation just verifying if java commands are available from the Terminal

```bash
java -version
----
openjdk version "11" 2018-09-25
OpenJDK Runtime Environment 18.9 (build 11+28)
OpenJDK 64-Bit Server VM 18.9 (build 11+28, mixed mode)
----
```


Thats it! The system is ready to use Java OpenJDK commands!
