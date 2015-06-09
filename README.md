offlineimap-daemon
==================

Script to run offlineimap only when network connection is present. This script
circumvents same problems with offlineimap, like offlineimap giving up syncing
when connection lost. This script also saves your CPU cycles.


requirements
------------

* python 3
* Network Manager
* offlineimap configured to run as daemon, i.e.


	[Account personal]
	autorefresh = 5
	quick = 10
	...


usage
-----

Simply setup `offlineimap-daemon.py` as daemon with your init system, run it
in your `.xinitrc` or in whatever way your system uses for starting user's daemons.

For convenience there is also `offlineimap-daemonctl.sh` control script.