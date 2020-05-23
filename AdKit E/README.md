# AdKit E

AdKit E adds non-intrusive ads to the bottom of vCard menus. It supports both iOS 12 and iOS 13.

- [Download the iOS 12 version](https://fifithebulldog.github.io/shortcuts/AdKit%20E/AdKit%20E.shortcut)
- [Downlaod the iOS 13 version](https://routinehub.co/shortcut/5369)

AdKit E helps provide your favorite shortcut creators with funds, so they can continue to make great shortcuts. AdKit E shows ads as a small, non-intrusive menu item.

AdKit E is easy for shortcut developers to use.

### 1. Make an ad unit with A-ADS

Go to https://a-ads.com and make a new ad unit, with the configuration as follows:

Type: App

Description: iOS Shortcut

Ad type: Adaptive, Mixed

### 2. Make a vCard menu

Create a vCard menu. If you don’t know how to do this, [here is an excellent tutorial](https://www.reddit.com/r/shortcuts/comments/aibvkg/creating_visually_appealing_menus/).

### 3. Add AdKit E to your shortcut

**Step 1:** Use a copy-and-paste shortcut such as [Copy And Paste A Shortcut](https://routinehub.co/shortcut/4118) by [@robric18](https://routinehub.co/user/robric18) to copy AdKit E to the top of your shortcut.

Paste a base64-encoded image into the text field that says "Paste base64 encoded ad icon here." This will be the icon for the ad in your vCard menu. You can use your own, or you can copy the encoded icon from the preceding Comment action and paste that into the icon field—that is the ad icon from the standalone version of AdKit.

Edit the "Run Shortcut" action near the bottom of AdKit E to run the shortcut containing it after you have copied AdKit E into your shortcut.

**Step Two:** Make a dictionary. The key-value pairs are as follows.

- "Function": (text) "AdKit"
- "ID": (text) The unit ID for your A-ADS unit.
- "Menu": (text) Put your vCard menu in a Text action before the dictionary and put the magic variable from that Text action in this field. AdKit E will attach an ad to the bottom of this menu and display it.
- "Prompt": (text) The prompt for your menu.

**Step Three:** Place a "Run Shortcut" action after the dictionary. Make sure the dictionary is the input for the Run Shortcut action, and choose the name of your shortcut so that your shortcut will run itself. Turn off "Show While Running."

Download an example shortcut to see how this should look:

- [iOS 12](https://fifithebulldog.github.io/shortcuts/AdKit%20E/AdKit%20E%20Example.shortcut)
- [iOS 13](https://www.icloud.com/shortcuts/954e803c7fed45e1934f46b9294b23a8)

That’s it! When users run your shortcut and need to display the menu, AdKit E will download an ad, append it to the bottom of the menu, and display the menu. If a user clicks the ad, the ad will open in Safari and your shortcut will wait for them to return to Shortcuts before continuing.
