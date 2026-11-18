# Diyelo Dulay — Portfolio

A personal portfolio built as a macOS-style workspace, in a single HTML file with no libraries and no build step.

**Live site:** https://diyel08.github.io

Diyelo Dulay is a Failure Analysis technician in Laguna, Philippines. The site covers his background, his experience and the tools he builds at the bench: calculators, simulators and learning labs for electronics, power and solar work.

## What is in it

- **Desktop workspace.** Every section opens as a window with a menu bar, a dock, desktop widgets and folders, Spotlight search, Quick Look, Mission Control, window tiling, Stage Manager, wallpapers and sound.
- **Portfolio apps.** README (welcome screen), About, Experience, Contact, CV, Skills, Guides, Finder (Icons, List and Columns views), System Settings and a changelog.
- **Applications.** Calculator (Standard, Scientific, Programmer and Electronics modes), Passwords (passphrase generator with QR), Budget (payday, bills, loans, savings goals, payments and backup), Reminders, Notes, Clock, Weather, Messages, Quiz and Links.
- **Simulators.** Breadboard, Motor Control, Schematics and Wiring.
- **Labs.** Analog, Audio, Bench, Drawing, Monitor and Solar. These are teaching tools with ideal-part maths, not designs for real installations.
- **Launchpad.** All apps grouped by type, with search (F4, the Go menu or Control Center).
- **Control Center and Notification Center.** Toggles for Dark Mode, Sound, Stage Manager, Widgets, Dock Magnify and Effects, brightness and volume sliders, accent colors and shortcuts. Notifications can be dismissed one by one.
- **Appearance.** Light, Dark or Auto, seven accent colors and several wallpapers, all in System Settings.
- **Phone Control Center.** On phones it opens full screen with round glass buttons, an accent tile, tall vertical Display and Sound sliders, a Focus list (Do Not Disturb, Reduce Interruptions, Personal, Work, Sleep) and shortcuts. Hold the Display slider for Dark Mode, Night Shift and True Tone. The power button opens a slide to power off screen.
- **Phone lock screen.** Large time, three widgets (day progress, next alarm, Focus) and a passcode keypad. Any 6 digits unlock the demo.
- **Clock and Calendar.** Clock has World Clock, Alarms, Stopwatch and Timers tabs. Calendar is a month grid with events saved in the browser.
- **Mail.** A compose form addressed to the public email. Send opens the visitor's own email app with the message filled in; the page sends nothing itself.
- **App Library.** The last page of the phone Home Screen groups all apps into Portfolio, Applications, Simulators and Labs cards.
- **Phones.** Below 700 px wide the site becomes an iPhone-style Home Screen with app icons, widgets and a dock. Apps open full screen, and Simulators, Labs and Applications sit in Home Screen folders.

## Keyboard shortcuts

| Keys | Action |
| --- | --- |
| `/` or `Ctrl K` | Open Spotlight search |
| `F3` or `Ctrl ↑` | Mission Control |
| `F4` | Launchpad |
| `Alt ←` / `Alt →` | Tile the front window to the left or right half |
| `Alt W` | Close the front window |
| `Alt M` | Hide (minimize) the front window |
| `Alt Z` | Zoom the front window |
| `Alt F` | Full screen for the front window |
| `Alt` + `` ` `` | Switch between open windows |
| `Space` | Quick Look on the selected file in Finder |
| `Esc` | Close the open menu, search, preview or panel |

Hot corners (turn them on or off in System Settings): top left opens Mission Control, top right opens Notification Center, bottom right shows the desktop.

## Phone gestures

- Tap **‹ Home**, tap the bar at the bottom, swipe up from the bottom edge or swipe right from the left edge to go back to the Home Screen.
- Pull down on the Home Screen to open Search.
- Swipe down from the top edge: the left half opens Notification Center, the right half opens Control Center.

## Run it locally

There is nothing to install. Open `index.html` in a browser, or serve the folder with any static server:

```
python3 -m http.server 5500
```

Then open `http://127.0.0.1:5500`.

## Project layout

```
index.html   the whole site: HTML, CSS and JavaScript
README.md    this file
```

The site is published with GitHub Pages from the main branch. To update it, edit `index.html`, check it in a browser, then commit and push.

## Browser support and known limits

- Built and tested in current Chromium-based browsers. Safari 16 (macOS Monterey) has not been tested yet.
- A browser cannot use `Alt Tab`, so the window switcher uses `Alt` and the backtick key.
- The glass effect is an approximation made with blur and gradients, not real refraction.
- In Dark mode the diagrams and the CV stay white on purpose, so they stay readable and the CV prints correctly.

## Privacy

The only public contact on the site is the email address shown on the Contact app. No phone number or home address is published. Settings (appearance, accent, wallpaper, sound) are stored in the visitor's own browser and are never sent anywhere.

## License

All rights reserved. See [LICENSE](LICENSE). Viewing the live site is welcome; copying or reusing the code, design or content needs written permission.

## Contact

Email: diyelodulay@gmail.com · GitHub: [Diyel08](https://github.com/Diyel08)
