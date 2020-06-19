![](demo/preview.gif)

# WM agnostic clear transparent workflow for Unix

No more ugly windows behind your beautiful transparent one

# Features

-  Can be used on any window manager
-  No background windows on fullscreen mode
-  No background windows on monocle mode
-  Navigation between hidden windows
-  Auto navigate to previews hidden window after closing

# Dependencies

-  A compositor(duh!)
-  xdo
-  wmctrl

# Prerequisites

-  Get the **WM_NAME** of your status bar using **xprop** and change the **STATUS_BAR** variable in the script accordingly

# Usage

```sh
crystal --toggle [monocle,fullscreen]  # toggle crystal mode
crystal --navigate [next,prev]         # navigate to next/prev hidden windows
crystal --close                        # closes current window and focuses on the previous one
```

# FAQ

### Your status bar looks cool! What's that!

![Uniblocks](https://github.com/salman-abedin/uniblocks)

### How are you launching those files and folders so fast!

![Bolt](https://github.com/salman-abedin/bolt)

### What is this sorcery of a system!

![Magpie](https://github.com/salman-abedin/magpie)

### You are so jazz! Where can I reach you!

SalmanAbedin@disroot.org
