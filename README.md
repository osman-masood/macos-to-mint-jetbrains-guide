# macos-to-mint-jetbrains-guide
Guide for macOS developers switching to Linux Mint, specifically users of Jetbrains IDEs (PyCharm, IntelliJ, etc.) Developed for Mint 18.1.

- Disable (or re-map) the Mint key bindings which interfere with the IDE: https://askubuntu.com/a/412060/67494 . In addition to these, you'll want to disable: 
  - Windows -> Tiling and Snapping -> everything in here
  - Windows -> Close window, Maximize window, Show desktop, Toggle maximization state
  - Launchers -> Home folder
  - Hardware -> Orientation lock, Re-detect display devices
  - General -> Run dialog, Run expo

- If you're using a PC with a `Win` key, swap the `Win` and `Meta` keys: https://askubuntu.com/a/692993 . This will allow you to use the Mac OS X 10.5+ keybinding, which on Linux uses `Meta` instead of `Command`. 

- In System Settings -> Windows -> Behavior tab, change "Special key to move and resize windows" to Disabled or Super. This is so you'll be able to use `Alt + Mouse1Click` in the IDE.

- If you're using a PC keyboard and your `Alt` key is where your Macbook's `Command` key was, you'll need to swap those two buttons in all Keymap commands in PyCharm. They Keymap file which does this is in this repo. Move this into `~/.PyCharm2017.1/config/keymaps/`, and load this Keymap up with PyCharm.
  - Note on the Keymap: I didn't map any numpad commands, nor "Next Project Window" or "Previous Project Window", since I don't know how to disable `Alt + Backtick` yet.

- For a macOS-style window menu bar, go to System Settings -> Windows -> Titlebar tab, and set "Left side title bar buttons" to Close, Minimize, and Maximize, in that order. 
