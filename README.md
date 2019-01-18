# nagios-check-gluster
Check volume, bricks and free space Gluster

Please file in your plugin directory /usr/lib/nagios/plugins

Requirements bc awk sudo pidof and ...... gluster

USAGE: 
  check_gluster.sh -v VOLUME -n BRICKS [-w GB -c GB]
     -n BRICKS: number of bricks
     -w and -c values in GB

Run check for example; /usr/lib/nagios/plugins/check_gluster.sh -v gvol14 -n 2 -w 1000 -c 500

Add check to your config.

Inspired by a script of Mark Nipper (seen first by Mark Ruys and modded by Erwin van den Bovenkamp in 2019)
