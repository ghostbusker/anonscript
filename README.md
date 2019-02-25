# anonscript
Designed for Raspberry Pi: randomizes network profile, creates reverse tunnel access with dynamic dns

On each reboot, or when manually running script, the following are erased and randomly regenerated:
Machine-ID
MAC addresses
Hostname

Additionally, the Pi requests a new UPNP pinhole for the selected port and attempts to update a dynamic DNS link to allow easy remote access.

*************
Needed improvements:

-try with different Pi models (currently tested working on Pi3b using ethernet)
-test UPNP compatibility with different routers
-add script to remove current UPNP mapping each time anonymizing script is run (to prevent conflict when Pi reconnects with new identity)
