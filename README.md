# astrosync
rsync for ASIAIR 

This is a simple script that can be used to copy images from an ASIAIR during the imaging session, similar to what the Robocopy plugin does in NINA. 

I can be run from cron, or it can be run from the command line.

If run from a command line, you can run it two ways:

1. with no arguments, in which case it will run rsync once and exit.
2. with --loop, in which case it will run rsync, wait 30 seconds and run again.

It checks both the EMMC Images folder and the TF Images folder, and copies their contents to whatever directory you configure in the script.  

The folder you wish to copy from must be mounted on '/Volumes/EMMC Images' or '/Volumes/TF Images', which are the default mount points for these shares when mounted.

You will need to edit the destination folders to your desired target location.
