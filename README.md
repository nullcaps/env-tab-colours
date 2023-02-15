# Environment-based tab colours
For Firefox and Vivaldi browsers only (sadly no CSS UI editing in Google Chrome or Safari).

## Vivaldi installation
### Enable custom CSS
See [https://forum.vivaldi.net/topic/10549/modding-vivaldi](https://forum.vivaldi.net/topic/10549/modding-vivaldi) for full instructions. Summary:

1. Open Vivaldi, and go to '**vivaldi://experiments**'
2. Enable '**Allow for using CSS modifications**'
3. Open appearance section in settings, then choose the folder to store your CSS files in
4. Paste customUI.css from this repo to chrome folder

### Whitelist domains in CSS
Open CSS file and edit the following:

1. The colours to use for your environments
2. The domains associated with each environment
3. Any subdomains you want to leave uncoloured

## Firefox installation
### Enable custom CSS
See [https://www.userchrome.org/](https://www.userchrome.org/how-create-userchrome-css.html) for full instructions. Summary:

1. Visit the default profile folder for Firefox. Usually: `~/Library/Application Support/Firefox/Profiles/<randomstring>.default-release/`
2. Create folder, name it '**chrome**'
3. Paste userChrome.css from this repo to chrome folder
4. (Optional) Open css and set a colour to use for non-container tabs
5. Open Firefox and go to '**about:config**'
6. In the search bar, enter 'userprof', find '**toolkit.legacyUserProfileCustomizations.stylesheets**', and set to true
7. Fully close Firefox and reopen

### Whitelist domains in Firefox containers
If you don't already have it, grab the Firefox Multi-Account  containers extension from [https://addons.mozilla.org/](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/)

Once the addon is installed, whitelist whichever domains you would like to be highlighted and select the colour to use from the addon menu.

**Recommended**: Enable 'limit to designated sites' to move out of the container when moving to a different domain

**Optional**: Open userChrome.css and change active-tab-colour
