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


## Contributing

Contributions of game configurations to this repository are welcomed and encouraged! There are two options for how to do this.

1. **Submit a pull request.** This requires using `git` commands to clone this repository, committing one or more changes, pushing the changes back to GitHub, and then creating a pull request on GitHub.

2. **Create an issue** using the "Configuration File Submission" issue template. Fill in the requested details and paste the proposed configuration file directly into the issue itself.

Option 1 is preferred and best for a higher number of configuration files, but option 2 is also available for those who are not familiar with `git` workflows or prefer something simpler.

Regardless of submission option, contributors listed as an author  on any submitted configurations will need to agree to license their contributions to me (samuelgr) under the same 3-clause BSD license that is used by this repository.


### Formatting Instructions

Configuration files in this repository must begin with a comment block at the top, with the configuration itself below it. The comment block identifies the game, Xidi form, tested Xidi version, authors, and so on.

Below is a template for the comment section at the top, which can be directly copied and pasted as an easy way of getting started.

```ini
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
; (application/game name here)
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
; Xidi Version:     (which Xidi version did you use for testing?)
; Xidi Form:        (which form of Xidi does this game use? - see instructions)
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
; Authors:          (comma-separated lsit of names/GitHub usernames for anyone who contributed)
; Last Modified:    (last edit date in M/D/YYYY)
;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
```

 - For **Xidi Version** use just the bare version, "4.1.1" for example. Only officially-released versions are allowed, not development or other one-off builds.
 - For **Xidi Form** indicate which form of Xidi is needed for this application. Pick one of the below, as appropriate.
    - `DInput`
    - `DInput8`
    - `WinMM`
    - `HookModule + DInput`
    - `HookModule + DInput8`
    - `HookModule + WinMM`

After the comment section comes **two blank lines** followed by the rest of the configuration file contents. Refer to the formatting of existing configuration files in this repository for specifics on formatting expectations regarding line spacing and formatting, but the general rule of thumb is **two blank lines between sections** and **one blank line between groups of related settings** such as element mapper configurations for related in-app controls.
