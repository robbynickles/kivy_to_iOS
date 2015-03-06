Command-line script that installs a kivy app to iOS. 

How to use:

./kivyToApp3.sh /path/to/your/kivy/project


The script assumes three things are installed on the host machine (the host machine is where kivyToApp3.sh is executed).
1) iproxy (for ssh via usb).
2) Apple Command-Line Tools 
3) ldid


The script also assumes some things about the XCode project template that your installation of kivy uses:
1) Either you have a code-signing identity, or code-signing is turned off.
2) You have the right SDK to build for your phone's version.

The best way to make sure the project template is setup correctly for you is to edit the file 'kivy-ios/tools/templates/template.xcodeproj/project.pbxproj'. The .pbxproj configures settings of an XCode project. 


