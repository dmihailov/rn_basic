# rn_basic
RN basic stuff; Start projects

# Environmental Variables Needed
(MAC) "user" - to be replaced with real user
export ANDROID_HOME=/Users/"user"/Library/Android/sdk
export ANDROID_AVD_HOME=/Users/"user"/.android/avd
export ANDROID_SDK_ROOT=/Users/"user"/Library/Android/sdk
export PATH="$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools:$PATH"
export PATH="$ANDROID_SDK_ROOT/emulator:$ANDROID_AVD_HOME:$PATH"

# Android Emulator Commands
*List of emulators:*<br/>
emulator -list-avds

*Run emulator:*<br/>
emulator @name_of_the_emulator

*ADB devices list:*<br/>
adb devices

*Kill emulator. "device_name" as in list of adb devices:*<br/>
adb -s device_name emu kill

*Open RN debug menu:*<br/>
adb shell input keyevent 82

*Reload RN app:*</br>
adb shell input text RR
