# ionic-scroll-issue

This is a demo ionic app which illustrates issue we are experiencing while developing our app.

**Type: bug**

**Platform: android 5.1.1 (webview 39.0.0.0)**

This is the native scrolling issue we are experiencing:

**Issue: native scroll (side menu) becomes frozen after using modal window**

Note: Native scrolling previously enabled using: $ionicConfigProvider.scrolling.jsScrolling(false).

**Situation:**

1. Open modal window (in this demo, this is ‘Login’)
2. Change orientation of the mobile device (while modal window is still opened)
3. Close modal window
4. Click to open side menu

Result is that we are unable to scroll through the side menu.

This issue also happened when in case when we weren’t changing the orientation of a device, but we used modal window to change appearance of our app (css, menu items etc.). I believe this is the same issue as the one demonstrated by this demo app.

I tested our app on following android versions: 4.1.2, 4.4.2, 5.0.1, 5.1.1, 6.0. As said, the issue occurred only on version 5.1.1.
