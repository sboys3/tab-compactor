# Firefox Tab Compactor


![Example Of Tabs](./doc/Screenshot%202024-04-17%20145356.png)

This is an extension that uses userChrome.css to allow tabs to significantly decrease in size in the toolbar.

I also recommend setting `browser.compactmode.show` to true in about:config and going into `more tools > customize toolbar` and setting the mode to compact for more space savings.


## Installation
This can be installed as a theme or as a userChrome.css file.

### UserChrome.css
To use this as a userChrome.css file, follow these steps:
1. Open Firefox's `about:config` page.
2. Find the `toolkit.legacyUserProfileCustomizations.stylesheets` preference and set it to true.
3. Create a new folder in your Firefox profile directory called `chrome`.
4. Inside the `chrome` folder, create a new file called `userChrome.css`.
5. Paste the contents of `userChrome.css` into this file.
6. Restart Firefox.

### Theme
To use this as a theme, follow these steps:
1. Be using a Nightly or Developer build of Firefox.
2. Follow the building extension instructions to create the extension zip file.
3. Set the about:config Options Required for Testing Theme.
4. Open Firefox's `about:addons` page and drag the zip file onto the page to install the theme.

## about:config Options Required for Testing Theme
Without these, Firefox will say the extension is corrupt and won't load. This also requires the nightly build of Firefox.
* xpinstall.signatures.required: false
* extensions.experiments.enabled: true


## Building Extension
Just zip up `manifest.json`, `userChrome.css` and `icons`.