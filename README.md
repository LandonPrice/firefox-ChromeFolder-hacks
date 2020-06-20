# firefox-ChromeFolder-hacks
A personal collection of CSS modifications to the Firefox web Browser. Many elements are still under development/modernization. Design langauge healivy utilizes an appealing copper orange (#c87553) on dark background theme.

![header](https://i.imgur.com/yU2lHO5.png)

# Loading user*.css files

0. Go to about:config and set the pref `toolkit.legacyUserProfileCustomizations.stylesheets` to `true` to make Firefox load userChrome.css and userContent.css

1. Find your profile folder, if Firefox is running you can find by going to `about:support` and there should be a button with label "Open Folder" under application basics
2. Create a new folder to the profile folder and name it "chrome"
3. `userChrome.css` and `userContent.css` files should be created inside this chrome-folder.

Clone this repository or individual files inside that newly created chrome-folder.
In the end you should have a folder structure like this:

```
<profile_folder>
|_chrome
|   |_ShadowFox_customization
|   |_userChrome.css
|   |_userContent.css
|_extensions
|_prefs.js
...
all other profile folders and files
...
```

In short, create a parent chrome folder to the same directory where `prefs.js` is - the main profile folder. Firefox loads `userContent.css` and `userChrome.css` files only from that `chrome`-folder.

## Customization

**the bars are at the bottom reeeeeeeeeeeeeeee**
 Its easy to customize the background and accent colors. Just edit the hex values in `ShadowFox_customization/colorOverrides.css`
 To Customize the various elements, remove or add the relevent code at the end of the `userChrome.css` file. Reading the comments are  your friend. Google-fu and searching https://old.reddit.com/r/FirefoxCSS/ will help. 

# Profile Configuration

Watch this tutorial on how to set the extentions/config that I use.

[![](http://img.youtube.com/vi/SgO-0p64OMQ/0.jpg)](http://www.youtube.com/watch?v=SgO-0p64OMQ "Firefox Customization")
 
# Credit to the following projects:

**Shadowfox Theme** - https://github.com/overdodactyl/ShadowFox (this is kind of a 'soft fork' of shadowfox)

**CSS-Hacks** - https://github.com/MrOtherGuy/firefox-csshacks
