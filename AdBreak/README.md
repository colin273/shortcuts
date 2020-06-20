# AdBreak

This is the iOS 12 version of AdBreak. [Download AdBreak for iOS 13 on RoutineHub.](https://routinehub.co/shortcut/5357)

Version: 1.2

Made with [ScPL](https://scpl.dev)

Stop ads from ruining the Shortcuts user experience.

[AdKit](https://routinehub.co/shortcut/5350) by [@eaic](https://routinehub.co/user/eaic) is a new tool that allows shortcut developers to inject ads into their shortcuts’ vCard menus. Right now, AdKit’s ads are relatively unintrusive, but there is no guarantee that they will stay that way.

So far, Shortcuts has been mostly free of ads and other such annoyances. It has consistently been a relief from the onslaught of ads that has taken over web and app development. Now AdKit threatens the happy absence of ads in Shortcuts.

This shortcut gets rid of ads delivered by AdKit. Instead of installing AdKit, you can install this to remove the ad injection process, and therefore block ads in Shortcuts. If you already have AdKit installed, press “Replace” when Shortcuts asks you if you wold like to overwrite AdKit. The AdBreak shortcut is named AdKit so that it can intercept all AdKit calls.

There is no loss of functionality for shortcuts that use AdKit (besides the ads themselves) when using AdBreak. In fact, any shortcuts that use AdKit will run faster with AdBreak.

Note: AdBreak only blocks ads if AdKit is used as an external dependency. If AdKit is embedded into a shortcut, then the only way to remove ads is to delete the AdKit actions or use a different shortcut.
