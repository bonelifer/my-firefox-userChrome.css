# my-firefox-userChrome.css

Personal `userChrome.css` setup for customizing Firefox's UI.

## Contents

| File | Purpose |
|---|---|
| `chrome/userChrome.css` | Entry point — imports all the files below. |
| `chrome/disable.css` | Hides the tracking-protection icon and disables its animation. |
| `chrome/findbar.css` | Moves the Find Bar above the page and repositions its border. |
| `chrome/overridemegabarenlargement.css` | Prevents the URL bar from enlarging ("megabar") on focus. |
| `chrome/remove_megabar.css` | Removes the megabar UI change entirely ([source](http://userchrome.wesleybranton.com/megabar)). |
| `chrome/roomybookmarks.css` | Recreates the Roomy Bookmarks Toolbar add-on's spacing for top-level bookmarks. |
| `chrome/scrollbars.css` | Widens scrollbars. |
| `chrome/soundicon-on-favicon.css` | Shows the tab audio icon overlaid on the favicon. |
| `chrome/urlbarfullheight.css` | Stretches tabs to the full height between the URL bar and window top. |
| `chrome/widget-overflow.css` | Tweaks the toolbar overflow menu. |

## Installation

1. Locate your Firefox profile folder (`about:support` → "Profile Folder").
2. Copy the `chrome/` folder from this repo into your profile folder.
3. In `about:config`, set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
4. Restart Firefox.

Comment out `@import` lines in `chrome/userChrome.css` to disable individual tweaks.
