http://forum.arduino.cc/index.php?topic=351999.msg2438295#msg2438295

## Problem ##

`no serial port name defined`

Arduino doesn't see USB serial port. 

## Solution ##

Need to disable kext driver signing checks.

1. Boot to recovery mode by holding Cmd-R during boot.
2. Type `csrutil enable --without kext` at cmd prompt
3. Reboot as normal

## Pitfalls ##

This configuration is unsupported and may leave the machine in a broken state at some point in the future.

