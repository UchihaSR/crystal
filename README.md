![](demo/preview.gif)

# Window manager agnostic clear transparent workflow for Unix

No more ugly windows behind your beautiful transparent one

This is the next iteration of
[Mono Trans BSPWM](https://github.com/salman-abedin/mono_trans_bspwm)

## Features

-  Can be used on any window manager
-  No background windows on fullscreen mode
-  No background windows on monocle mode
-  Navigation between hidden windows
-  Auto navigate to previews hidden window after closing

## Dependencies

-  tail, xargs, shift
-  A compositor( ex. **xcompmgr, picom** etc )
-  [xdo](https://github.com/baskerville/xdo)
-  [xdotool](https://github.com/jordansissel/xdotool)

## Installation

```sh
git clone https://github.com/salman-abedin/crystal.git && cd crystal && sudo make install
```

## Usage

-  Get the **WM_NAME** of your status bar using **xprop** and create an environment variable named **STATUSBAR** accordingly.

   For example, put the following in your **.profile/.xprofile** if you are using yabar

```sh
export STATUSBAR=yabar
```

-  Restart

-  Bind these commands to your preferred key combinations

| Command                              | Effect                                                       |
| ------------------------------------ | ------------------------------------------------------------ |
| `crystal --toggle [solo,fullscreen]` | Toggles crystal mode on fullscreen or solo mode              |
| `crystal --navigate`                 | navigates between hidden windows                             |
| `crystal --close`                    | closes the current window and focuses on the last hidden one |

## Uninstallation

```sh
sudo make uninstall
```

## FAQ

### What if I change my status bar?

Change the **STATUSBAR** environment variable and you are good to go.

---

## Repos you might be interested in

[Bolt](https://github.com/salman-abedin/bolt)
: The lightning fast workflow creator

[Uniblocks](https://github.com/salman-abedin/uniblocks)
: The statusbar

[Magpie](https://github.com/salman-abedin/magpie)
: The dotfiles

[Alfred](https://github.com/salman-abedin/alfred)
: The scripts

[Devour](https://github.com/salman-abedin/devour)
: Terminal swallowing

## Contact

SalmanAbedin@disroot.org
