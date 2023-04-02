# AutoHotkey Keyboard Locker

This is an AutoHotkey script you can use to temporarily block keyboard input. When your keyboard is locked by this script, keypresses will be caught by the script and blocked, until you unlock your keyboard again.

# What is it for?

This fork edits the original repo to fit my needs, so that I can use it to lock/unlock the keyboard while using a pentablet to take notes
(desks are small so I need to use my pentablet on top off the laptop keyboard). Running the script multiple times will cycle between lock 
and unlock, so that I can just bind it in the pentablet software and press a button.

Note: This is not security software and is easily bypassed. Only use it for convenience, not security.

# How to use it

You can only run the script itself by forking the repo.

## Running the .ahk script

1) Install [AutoHotkey](https://www.autohotkey.com/) version 1.x in order to run .ahk scripts. Not tested with AutoHotkey version 2.
2) Fork the repo where you want.
3) Bind `keyboard-locker.ahk` in your pentablet software to a button.
4) Press the button to lock/unlock.

# Settings

Various settings can be changed by editing `settings.ini`. You can change the following settings.

- enable the keyboard shortcut or password
- change the keyboard shortcut or password
- enable tray notifications
- disable automatically lock on open
- disable automatically exit on unlock
- lock the mouse as well

The settings file contains explanations for each setting.

# Known issues

- Some media keys or Windows shortcuts may not be blocked.
- Some keys (especially modifiers) may get "stuck" after unlocking, requiring you to press them again to get them "unstuck".
- There is sometimes a slight delay after typing the password before the keyboard is unlocked.

Feel free to submit a PR if you have improvements for these issues!

# Potential future improvements

- Stealth mode: hide the tray icon and disable tooltips on lock, making it slightly more difficult to bypass the script.
- Temporary password: change the password at run time to avoid using the one that is readable in the script itself.
- Unlock timer: automatically unlock after a period of time.
- Inactivity lock: automatically lock after a period of inactivity.
- Scheduled lock: automatically lock and unlock on a schedule.

# Credits

The original repo obv.

This script is inspired by the Keyboard Locker script from this HowToGeek [article](https://www.howtogeek.com/howto/11570/disable-the-keyboard-with-a-keyboard-shortcut-in-windows/), which in turn was based on a script by an AutoHotkey forum user named Lexikos (the original forum thread appears to be lost due to forum move, but was originally found [here](http://www.autohotkey.com/forum/post-147849.html#147849)).
