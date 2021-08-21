# GSS_Submitter

An example client for GameScoreService API

# About

The application is coded in [Hollywood](https://www.hollywood-mal.com/index.html) 9.0, which is a Lua based scripting language, but which also offers options to compile scripts as applets that can be run with the [Hollywood Player](https://www.hollywood-mal.com/download.html) application or even as stand-alone executables for about 15 different platforms.

# Requirements

- [RapaGUI plugin](https://www.hollywood-mal.com/download.html) (not needed on Android)
- [hURL plugin](https://www.hollywood-mal.com/download.html)
- On Linux platforms: OpenSSL 1.0.x (1.1.x won't work)
- Operating system specific requirements can be seen [here](https://www.hollywood-mal.com/docs/html/hollywood/Requirements_.html)

**Note:** When running provided pre-compiled executables, the plugins are linked in the executable files and installation of them is not required!

# Running

There are three options to run the client application.

1. If you have the Hollywood development environment installed, just use the Hollywood interpreter to run the script file:  
```hollywood gss_submitter.hws```
2. Run a compiled applet in Hollywood Player on any of the supported platforms (plugin installation may vary depeding of the platform. For example, on Android it must be placed in the Hollywood/Plugins/ directory found on your device's internal storage or SD card after installation of the player).
3. Run a pre-compiled executable (provided for Windows (x64) and Linux (x64/GTK3) in this example project), this is the easiest solution.

# Configuring

After launching the application, configuration options can be found from the *File/Settings...* drop-down menu entry. The API server address, entry point path, and user (player) credentials can be changed from there.

# Usage

Click the *Home* button to access the API entry point, and then select the next action from control buttons at the bottom. Resource items can be accessed by single-clicking them on the *Items* list and the *Parent* button takes you back to the previous resource in the hierarchy tree.

User (player) specific actions do use the configured player information. Adding a new player will try to add the player with the configured information, as well as adding or editing scores.
