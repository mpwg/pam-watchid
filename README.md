PAM WatchID
-----------
A PAM plugin for authenticating using the new kLAPolicyDeviceOwnerAuthenticationWithBiometricsOrWatch API in macOS 12, written in Swift. Updated to be an universal binary (**ARM/Apple Silicon version untested**)

![](demo.gif)

Installation
------------

1. `$ sudo make install`
2. Edit `/etc/pam.d/sudo` to include as the **first** line: `auth sufficient pam_watchid.so "reason=execute a command as root"`

_Note that you might have other `auth`, don't remove them._
