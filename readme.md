Creating a google play release of the jpa:

Ensure that `platforms/andoird/project.properties` has these values:

key.store=cc-release-key.keystore
key.alias=cc_release_key


Resources for OSX (icons & Splash screens.):  
* include Images.xcassets in the Resources folder in x-code
* with Images.xcassets selected in the navigator on the left,
check off 'target membership' in the file inspector on the right.

If you get an error message about Cordova/CDVViewController.h file not found in
Xcode 7.x then you will want to Add this line to your
Build Settings -> Header Search Paths:

       "$(OBJROOT)/UninstalledProducts/$(PLATFORM_NAME)/include"

From [iconic forums](http://forum.ionicframework.com/t/cordova-cdvviewcontroller-h-file-not-found-in-xcode-7-1-beta/32232/5)
