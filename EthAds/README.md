EthAds adds non-intrusive ethical ads to the bottom of vCard menus.

## What are “ethical ads”?

An ethical ad doesn’t track users and is selected by the developer of the shortcut that displays it. These ads run for a set time and then go away.

## How does EthAds avoid tracking?

EthAds caches ads in iCloud Drive. Each ad has an expiration date, so once an ad has been downloaded, EthAds will not check for a new ad until the current ad has expired. This minimizes server exposure and helps EthAds run very fast.

## Where do ads for EthAds come from?

EthAds doesn’t use an external ad network; instead, it downloads its ads from a location controlled by you, the shortcut developer. I recommend using [GitHub Pages](https://pages.github.com/) for this; it’s fast, it’s free, and it’s relatively user-friendly. If you have your own website, you could also use that to host ads.

You will need to devise your own method for selling ad space to interested parties.

## How do I format ads on the server?

Ads for EthAds are formatted as a JSON. EthAds checks a master ad JSON on your site, which contains all the ads that you plan to run or have run in the past. EthAds will use the current date to determine which ad it needs to save and display, so you don’t need to worry about deleting ads as soon as they expire.

Here’s an example of what the ad file on the server might look like: 
File location: `https://example.com/ads.json`
```
[
    {
        "enddate": "2020-07-04",
        "title": "Hello World",
        "description": "Foo bar baz",
        "iconurl": "https://example.com/ad1.png",
        "website": "https://apple.com"
    },
    {
        "enddate": "2081-01-01",
        "title": "Lorem Ipsum Dolor",
        "description": "Sit amet",
        "iconurl": "https://example.com/ad2.png",
        "website": "https://routinehub.co"
    }
]
```

Note that the icons are not stored in the JSON as base64. Instead, their URLs are provided so that only the icon of the currently running ad will be downloaded.

Also notice that the expiration dates are in the ISO 8601 format to ensure that they are interpreted correctly regardless of the language and region settings of users’ devices.

## How do I add EthAds to my shortcuts?

Use a copy-and-paste shortcut such as [Copy And Paste A Shortcut](https://routinehub.co/shortcut/4118) by [@robric18](https://routinehub.co/user/robric18) to copy EthAds to the top of your shortcut.

There are several comments throughout EthAds that explain how to configure it. You can delete those comments when you have finished configuring EthAds.

EthAds is based on [AdKit E](https://routinehub.co/shortcut/5369), another ad-delivery system for Shortcuts that uses A-ADS instead of ethical ads.
