# android-ducky
Rubber Ducky with Android

# What is this repository for ?
* Android version of the famous Rubber Ducky
* Supports non-US keyboard layouts

# How do I get setup ?
* Root you android device
* Check this link for device specific procedure : https://github.com/pelya/android-keyboard-gadget
* Basically you will have to flash a new kernel to add HID keyboard support. Be sure to have TWRP or CWM Recovery otherwise the flashing process might not even start. If you don't have TWRP or CWM Recovery, you can simply download the appp Rashr. This requires root though.
* You will need a terminal emulator, I recommend that you install Terminal IDE from the Play Store with Hacker's Keyboard (otherwise the app will crash for Android > 4.4). But you can also use JuiceSSH or whatever.
* You will need cool payloads : https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payloads
* chmod +x hid-gadget-test
* chmod +x droidducky.sh

# Usage
* bash droidducky.sh payload.txt
* In the futur, you will be able to specifiy the keyboard layout as parameter

# Contributions guidelines 
* Add support for your country keyboard layout by editing the "convert" function in droidducky.sh
* If a specific key is not available at the moment, you can submit the issue by telling me what the name of key is with its scancode
* Scancodes for HID keyboard can be found here : http://www.hiemalis.org/~keiji/PC/scancode-translate.pdf


#Sources
* The original droidducky.sh script is taken from https://github.com/anbud/DroidDucky
* The original hid-gadget-test is taken from https://github.com/pelya/android-keyboard-gadget
