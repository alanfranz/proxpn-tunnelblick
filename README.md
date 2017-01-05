proxpn-tunnelblick
==================

This repository contains setting files (*.tblk) for Tunnelblick/OpenVPN appropriate for use with proXPN OpenVPN service,
along with the python script that can be used to generate them.


These settings were derived from the sample OpenVPN configuration files with information extracted from the proXPN branded Tunnelblick client.

These settings were created due to issues using the branded proXPN client on Macintosh OS X 10.9.5.

For more information and background on the original project (this is a fork) please visit https://paretech.wordpress.com/2014/12/14/proxpn.

## Installation
1. Verify that Tunnelblick is installed.
2. Verify that Tunnelblick has been executed at least once before proceeding.
3. If Tunnelblick is running, terminate/execute the program.
4. Copy the *.tblk files to ~/Library/Application Support/Tunnelblick/Configurations or open each config with Tunnelblick (for example by double clicking each one and following onscreen menus).
5. Start Tunnelblick.
6. Click on the Tunnelblick icon by the "Spotlight Icon" and select the desired server. 
7. Follow onscreen instructions.
8. If all went well, do internet connected things as normal (but now safer).

## Notes
1. These configuration files have been tested on a system running Macintosh OS X 10.9.5 and Tunnelblick 3.4.2 (build 4055.4161)
2. The first time a configuration file is used from within Tunnelblick, the operator may be prompted by Tunnelblick for their password so that the permissions set on the configuration files can be changed. This prompt has nothing to do with these configuration files, it is how Tunnelblick operates.
3. Users can save their proXPN password to the OS X keychain manager. At this time the password must be stored once for each configuration file or if the file name changes.
4. These configuration files attempt to downgrade privileges after initializing for security. As such Tunnelblick may display a warning: "Use 'down-root' plugin for OpenVPN?" Responding with either "Always use the plugin" or "Do not use the plugin" seems to work. Consequences of responding "Always use the plugin" are not known at this time. No issues have occurred by responding "Do not use the plugin" but that response has only been tested on a stable internet connection where Tunnelblick is not trying to automatically reconnect.
5. The path ~/Library/Application Support/Tunnelblick/Configurations may be hidden. If you want hidden files to be displayed Google for the answer, if this is a one time thing open terminal and use the following command: "open ~/Library/Application\ Support/Tunnelblick/Configurations".
