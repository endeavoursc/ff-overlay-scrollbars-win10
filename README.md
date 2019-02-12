# Firefox Quantum (57+) overlay scrollbars Win10-style      

![Screenshot Overlay Scrollbar](https://raw.githubusercontent.com/endeavoursc/firefox-overlay-scrollbars-win10/master/screenshots/screenshot.png)  
Overlay Scrollbar


![Screenshot Overlay Scrollbar On Mouse Hover](https://raw.githubusercontent.com/endeavoursc/firefox-overlay-scrollbars-win10/master/screenshots/screenshot-hover.png)  
Overlay Scrollbar on mouse hover


## What does this do?

These files replace the native Windows scrollbars inside Firefox Quantum for overlay scrollbars similar to those used in UWP Windows 10 native applications.

Unlike similar versions of this script, these scrollbars trigger their functionality even on the outermost pixels between the scrollbar and the edge of the browser window.
The animation is also different to other versions, so this one is less prone to blinking while switching between normal mode and mouse hover mode.

Please notice that this is based on a workaround which allows you to run arbitrary javascript in your browser context, as used to be enabled by the extension [userChromeJS](http://userchromejs.mozdev.org/).
While it currently works as intended, it may stop working on future versions of Firefox.

This mod does not involve adding any extensions, and instead works only by adding (or changing) files in your Firefox user profile.


## Installation

Place the three `userChrome.*` files in a `/chrome` directory [inside your Firefox profile](https://support.mozilla.org/en-US/kb/profiles-where-firefox-stores-user-data). If you already have a `userChrome.css` file, you may instead add the contents of the file here anywhere in your existing file.

To uninstall, remove the three files. If you have other content in the `userChrome.css` file you can remove just the part that you added during installation.

## Updating .js file

If you are updating or changing the [userChrome.js](https://github.com/endeavoursc/firefox-overlay-scrollbars-win10/blob/master/userChrome.js) file you need to clear the Firefox cache by deleting your profile inside *%UserProfile%\AppData\Local\Mozilla\Firefox\Profiles* (Windows)
This won't erase your settings, active sessions, etc.
