# FirefoxMaterialYou

A customized `userChrome.css` theme that brings Google's Material You 3 dynamic color scheme to Firefox on Windows. It extracts and applies your Windows accent color to the browser interface, creating a cohesive OS-integrated visual experience.


## Features

* **Material You 3 Dynamic Coloring:** Automatically adapts the browser's theme colors based on your Windows accent color.
* **Redesigned Toolbar Buttons:** Updated hover effects on toolbar buttons to sleek, modern circles, while keeping the rest of the native UI intact.
* **Windows 11 Integration:** Designed to work beautifully with Windows 11's modern design language.
* **This theme uses the Windows accent color as the base palette. For best results, enable automatic accent color from wallpaper in Windows Settings.
* 
## System & Compatibility

* **OS:** Windows 11 (Recommended)
* **Firefox Version:** Tested on **Firefox v152.x** (Dark Mode)

## Design philosophy

* Preserve Firefox's native layout whenever possible.
* Only restyle frequently used UI elements.
* Hide rarely used controls instead of maintaining custom styles for them.

---

## Prerequisites (Firefox Configuration)

To ensure the Mica backdrop and native theme accents apply correctly, you must enable several experimental flags in Firefox.
Firefox updates may change internal UI selectors and break parts of the theme.

1. Open Firefox and type `about:config` in the address bar.
2. Search for and set the following preferences to **`true`**:

| Preference | Value | Description |
|---|---:|---|
| `widget.windows.mica` | `true` | Enables Mica backdrop on Windows 11. |
| `widget.windows.acrylic` | `true` | Enables Acrylic blur where available. |
| `widget.windows.win11_theme_accent` | `true` | Uses the Windows 11 system accent color. |
| `browser.tabs.drawInTitlebar` | `true` | Allows custom title bar / Mica rendering. |

---

## Installation

1. Open Firefox and navigate to `about:support`.
2. Find the **Profile Folder** entry and click **Open Folder** (or *Show in Finder/Explorer*).
3. Inside your profile directory, create a new folder named `chrome` (if it doesn't already exist).
4. Download the `userChrome.css` from this repository and place it into the `chrome` folder.
5. In `about:config`, make sure the following flag is also set to **`true`**:
   * `toolkit.legacyUserProfileCustomizations.stylesheets`
6. Restart Firefox to apply the changes.

## Structure
- `userChrome.css` - Main entry file
- `modules/` - Modular CSS components used by the theme

## Known Issues
- Light mode has not been tested.
- Firefox UI changes may break selectors after updates.
- Requires Windows 11 accent color / Mica support for the intended look.

---

## License

This project is open-source and available under the [MIT License](LICENSE).
