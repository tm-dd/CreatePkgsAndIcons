# CreatePkgsAndIcons

A script to create packages from Apps (or folders) for macOS (X). 
On Apps with icons, the script tries to export the icons as PNG files.
You can use the icons in you Munki repository ( if copyright holder allows that ;-) ).

# How to use:

Install and configure:

* copy the script an config file to the folder with your Apps
* change the config file

Advanced option:

* you can define separated settings for Apps in the same folders

Example config file for the App "Jami.app" to define a version number like: 1.0.0.2020.02.12.1005

	sh-3.2$ ls -ld1 Jami.app
	Jami.app
	sh-3.2$ cat _build_files/Jami/create.cfg 
	VERSION='1.0.0.'$(date '+%Y.%m.%d.%H%M')
	sh-3.2$ 

PLEASE NOTE, YOU USE THE SCRIPTS ON YOUR OWN RISK.

Thomas Mueller <><
