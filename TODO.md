## Features
* Video: Start/Stop/Select Input
* Custom command (not sure how)

## Enhancements
* Camera preset not CE8+ compatible, need to switch APIs based on firmware
* Parse response XML for errors
* Mute Toggle support (includes compatibility needs for older versions that don't have a native command)

## TE4 support
* E20 won't take DTMFSend because it's looking for a CallID. Maybe not worth doing right now, but it's possible
  that going forward it may be worth enumerating the calls and picking one. Call ID can be found in 
  http://<ip>/getxml?location=Status/Call
* ResetTimer needs to be changed for TE4 (Standby/Reset)


## Longer term
* Build polling support for feedback
* Autogenerate API calls from device configuration
