# Xidi Game Configurations

This repository contains game-specific configuration files for use with [Xidi](https://www.github.com/samuelgr/Xidi). Each configuration file includes a recommended mapper configuration as well as documentation on how best to get the game working with Xidi.


## Using

To use the configuration files contained in this repository:

1. Download the [latest release](https://github.com/samuelgr/Xidi/releases) of Xidi.

1. Look through the [GameConfigurations directory](https://github.com/samuelgr/XidiGameConfigurations/tree/master/GameConfigurations) in this repository for the desired game title.

1. Examine the configuration file, named `Xidi.ini`, contained within for information on which version and form of Xidi is needed.
   - Typically the version needed will be at least v3.0.0.
   - Form will be either DInput, DInput8, WinMM, or HookModule + one of the other forms. See [Forms of Xidi](https://github.com/samuelgr/Xidi#forms-of-xidi) for more information on how to install the different forms of Xidi.

1. Download the configuration file and place it into the same directory as the game's form of Xidi.
   - For example, if the game executable is located at `C:\MyFancyGame\App.exe` and the form of Xidi is located at `C:\MyFancyGame\dinput8.dll` then the configuration file would be `C:\MyFancyGame\Xidi.ini`.
   - See [Configuring Xidi](https://github.com/samuelgr/Xidi#configuring-xidi) for more information on configuration files and where they should be placed.
