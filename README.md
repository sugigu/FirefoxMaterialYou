# FirefoxMaterialYou

A customized `userChrome.css` theme that brings Google's Material You 3 dynamic color scheme to Firefox on Windows. It extracts and applies your Windows accent color to the browser interface, creating a cohesive OS-integrated visual experience.

## Features

* **Material You 3 Dynamic Coloring:** Automatically adapts the browser's theme colors based on your Windows accent color.
* **Redesigned Toolbar Buttons:** Updated hover effects on toolbar buttons to sleek, modern circles, while keeping the rest of the native UI intact.
* **Windows 11 Integration:** Designed to work beautifully with Windows 11's modern design language.

## System & Compatibility

* **OS:** Windows 11 (Recommended)
* **Firefox Version:** Tested on **Firefox v152.x** (Dark Mode)
* *Note: Light Mode has not been fully tested yet.*

---

## Prerequisites (Firefox Configuration)

To ensure the Mica backdrop and native theme accents apply correctly, you must enable several experimental flags in Firefox.

1. Open Firefox and type `about:config` in the address bar.
2. Search for and set the following preferences to **`true`**:

| Preference Name | Value | Description |
| :--- | :--- | :--- |
| `widget.windows.mica` | `true` | Enables the Mica backdrop effect on Windows 11. |
| `widget.windows.acrylic` | `true` | Enables the Acrylic blur effect (if applicable). |
| `widget.windows.win11_theme_accent` | `true` | Forces Firefox to utilize the Windows 11 system accent color. |
| `browser.tabs.drawInTitlebar` | `true` | Essential for rendering the custom title bar and Mica effects properly. |

---

## Installation

1. Open Firefox and navigate to `about:support`.
2. Find the **Profile Folder** entry and click **Open Folder** (or *Show in Finder/Explorer*).
3. Inside your profile directory, create a new folder named `chrome` (if it doesn't already exist).
4. Download the `userChrome.css` from this repository and place it into the `chrome` folder.
5. In `about:config`, make sure the following flag is also set to **`true`**:
   * `toolkit.legacyUserProfileCustomizations.stylesheets`
6. Restart Firefox to apply the changes.

---

## License

This project is open-source and available under the [MIT License](LICENSE).
