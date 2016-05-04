# Introduction #

This page explains how to build the project in eclipse. If you haven't used eclipse or programmed for android before, please see the [Android Eclipse tutorials](http://developer.android.com/)

# Checking Out the Code #

  * Install [Subclipse](http://subclipse.tigris.org/), the subversion plugin for eclipse.
  * In Eclipse, go to Window -> Open Repository -> Other... and select "SVN Repository Browsing"
  * In SVN Repositories, right-click, New -> Repository Location, and add "http://boxeeremote.googlecode.com/svn/trunk/". Use https:// if you plan on making commits, as http:// will not work properly for this purpose.
  * Expand the new repository, and right-click on "Boxee Remote" and select Checkout. The defaults should be fine, so press OK.

# Running #

Run it as you would a normal android project. One trick is that you need to disable the "Require Wifi Connection" preference in the BoxeeRemote application, since the emulator pretends that it's on a mobile network, not wifi.

If you want to install it on your phone, you'll need to sign the package with your own key (see the [Android instructions on signing your application](http://developer.android.com/guide/publishing/app-signing.html)). Since your key isn't the same as the official one, you should uninstall the version of Boxee Remote you downloaded from the marketplace first.

# Fixing common build problems #
  * Ensure that you have the Android SDK installed.
  * Ensure that you have selected a build target. In eclipse, go to the Package Explorer and find your Boxee Remote project. Right-click on it and select "Properties". In the Properties window, select "Android" on the left side. You can then select a Project Build Target on the right side. Choose "Android 1.1" or the most appropriate option provided by the SDK, and Apply it. Click OK.
  * You may need to fix the Android project properties. Right click on your Boxee Remote project, select "Android Tools", and then "Fix Project Properties". You may have to do this again if you revert your project through Subversion.