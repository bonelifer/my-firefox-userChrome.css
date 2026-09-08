# my-firefox-userChrome.css

Personal `userChrome.css` setup for customizing Firefox's UI.

## Contents

| File | Purpose |
|---|---|
| `chrome/userChrome.css` | Entry point — imports all the files below. |
| `chrome/userContent.css` | Content-page stylesheet, loaded automatically by Firefox (not `@import`ed). Currently keeps scrollbars visible on youtube.com. |
| `chrome/audio-tab-mute.css` | Hides the tab audio icon on unselected tabs and highlights it when playing/muted. |
| `chrome/compact_about_config.css` | Makes the `about:config` list more compact. |
| `chrome/compact_proton.css` | Shrinks Proton UI spacing (toolbar buttons, tabs, menus) back toward the old compact mode. |
| `chrome/disable.css` | Hides assorted UI chrome (tracking-protection icon, hamburger menu, Page Actions, Firefox View, Profiles menu, etc.). |
| `chrome/findbar.css` | Moves the Find Bar above the page and repositions its border. |
| `chrome/fullheight-tabs.css` | Makes tabs square and stretches them to the full height of the tab bar. |
| `chrome/overflow.css` | Makes extension icons in the overflow/unified-extensions panel more compact. |
| `chrome/private-browser.css` | Hides the "Private Browsing" text label while keeping its icon. |
| `chrome/roomybookmarks.css` | Recreates the Roomy Bookmarks Toolbar add-on's spacing for top-level bookmarks. |
| `chrome/scrollbars.css` | Widens scrollbars and sets scrollbar color (width is also controlled via `widget.non-native-theme.scrollbar.size` in `about:config`). |
| `chrome/tab-group-editor.css` | Hides Tab Group options from the tab context menu. |

## Installation

1. Locate your Firefox profile folder (`about:support` → "Profile Folder").
2. Copy the `chrome/` folder from this repo into your profile folder.
3. In `about:config`, set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
4. Restart Firefox.

Comment out `@import` lines in `chrome/userChrome.css` to disable individual tweaks.


## License

This project is licensed under the **GNU General Public License v3.0**.

See [LICENSE](LICENSE) for more information.
