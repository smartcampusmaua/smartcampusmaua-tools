# [  Android Studio  ]

## Install Android Studio

*From: https://developer.android.com/studio?hl=pt&gclid=Cj0KCQjwmuiTBhDoARIsAPiv6L-ms5Fg_UWFNAVE1xEcFZ7F79KksC7MZqkDNbj7efsKuVbnwlKJ_m8aAgRjEALw_wcB&gclsrc=aw.ds*

Download the Linux x64 binarries at https://developer.android.com/studio?hl=pt&gclid=Cj0KCQjwmuiTBhDoARIsAPiv6L-ms5Fg_UWFNAVE1xEcFZ7F79KksC7MZqkDNbj7efsKuVbnwlKJ_m8aAgRjEALw_wcB&gclsrc=aw.ds website

Move the `tar.gz` file to the ~/smartcampusmaua/smartcampusmaua-tools/Android/src directory
```bash
mkdir -p ~/smartcampusmaua/smartcampusmaua-tools/Android/src
mv ~/Downloads/android-studio-*.tar.gz ~/smartcampusmaua/smartcampusmaua-tools/Android/src
```

Uncrompress the android-studio-* file at the ~/Tools/Android/ directory
```bash
cd ~/smartcampusmaua/smartcampusmaua-tools/Android/src
tar -vxf android-studio-* -C ../
```

Open the ~/.bashrc file and include the android-studio binaries in the environment variable called PATH in the last lines of this file.

Open the `~/.bashrc` or `~/.zshrc` file and include the Nodejs binaries in the environment variable called PATH in the last lines of this file configure the Linux Terminal default options.
```bash
nano ~/.bashrc
# or 
nano ~/.zshrc
```

Then, add in the last line of the file:
```bash
# Set android-studio binaries to the PATH
export PATH=$PATH:~/smartcampusmaua/smartcampusmaua-tools/Android/android-studio/bin
export ANDROID_HOME=~/smartcampusmaua/smartcampusmaua-tools/Android/SDK
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
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
studio.sh
```

Then configure the SDK instalation directory to match the `$ANDROID_HOME` environment variable: `~/smartcampusmaua/smartcampusmaua-tools/Android/SDK`


In order to use the Android Phone as debugging tool, it must to enable `Developer Options` and turn `USB Debugging` on in the Phone Configuration.

Thats it! The system is ready to use Java JDK commands!
