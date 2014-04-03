eyetv2plex
==========

Copy files from EyeTV Archive to Plex Folder

This project is heavily inspired by https://github.com/miyagawa/eyetv-plex/blob/master/eyetvscan 

This project is especially useful when used with Plex plugins:

 * Extended Personal Media Agent [https://forums.plex.tv/index.php/topic/83440-rel-extended-personal-media-shows-agent/]
 * Extended Personal Media Scanner [https://forums.plex.tv/index.php/topic/88982-rel-extended-personal-media-scanner/]

When used with these two plugins, I needed a few more features:

 * Should generate .summary files from the information saved in .eyetvr xml file
 * Should copy files instead of just linking, as I wanted to move recordings away from HTPC to NAS
 * Some MPEGs saved by EyeTV was found to be "broken", ie. Plex couldn't fastforward in files, info was incorrect etc, so uses FFMPEG copy instead of OS copy
 * Should only copy files that are X days old
 
Using this script requires the following (on a Mac OS X Mavericks):
 
 * Install ffmpeg from macports (http://www.macports.org)
 * Install rubygem
 * Install Gems: streamio-ffmpeg, plist
 
This script is not widely tested, so use at own risk.  
