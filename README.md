# Diyelo Dulay — Portfolio

A personal portfolio built as a macOS-style workspace, in a single HTML file with no libraries and no build step.

**Live site:** https://diyel08.github.io

Diyelo Dulay is a Failure Analysis technician in Laguna, Philippines. The site covers his background, his experience and the tools he builds at the bench: calculators, simulators and learning labs for electronics, power and solar work.

## What is in it

- **Desktop workspace.** Every section opens as a window with a menu bar, a dock, desktop widgets and folders, Spotlight search, Quick Look, Mission Control, window tiling, Stage Manager, wallpapers and sound.
- **Portfolio apps.** README (welcome screen), About, Experience, Contact, CV, Skills, Guides, Finder (Icons, List and Columns views), System Settings and a changelog.
- **Applications.** Calculator (Standard, Scientific, Programmer and Electronics modes), Passwords (passphrase generator with QR), Budget (payday, bills, loans, savings goals, payments and backup), Reminders, Notes, Clock, Weather, Messages, Quiz and Links.
- **Simulators.** Breadboard, Motor Control, Schematics, Wiring and Sound Room.
  - Sound Room (sound.sim): pick a 2.0 to 7.1 layout or add speakers, drag them (and the listener) around a top-down room, and read each speaker's distance, angle, delay, trim and cable run. Turn Sound on to hear it with Web Audio: tap a speaker for noise, run Calibrate, or play the Demo. Headphones give the best 3D effect. It is a teaching model, not a room-acoustics simulation.
  - Breadboard editing: drag a placed part to move it (a selected group moves together), Shift-tap, Multi or box-select for several, Delete or Backspace to remove, arrow keys to nudge, Undo/Redo (Ctrl+Z), and Clear (undoable).
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

## Electrical apps (Build 78)
- **Motor Control** has five circuits: DOL, jog/run, forward/reverse, star-delta and hand-off-auto. Live amps (with starting inrush) and rpm show in the status bar. Insert a fault (open fuse, stop chain or coil, welded pole, lost phase, or a random hidden one), read the 230 V control circuit with the meter, and tick off the commissioning checklist. Save diagram downloads the ladder and power circuits as one SVG.
- **Wiring** adds a Voltage drop calculator (single or three phase, copper or aluminium, 3 % and 5 % limits) and a Fault finding bench with a meter (reversed polarity, open neutral, open earth, loose live joint) that shows why you test under load.

## Phone iOS 27 layout (Build 79)
- Status bar order: signal bars, 5G, Wi-Fi, battery with percentage (real level where the browser exposes it; Safari does not, so it shows 90). Same on the lock screen.
- Swipe down from the top-left half of the status bar for the notification screen (big time, date, widgets, calendar, notifications); from the top-right half for Control Center. The panel follows the finger. Tapping the clock or the signal/Wi-Fi/battery icons does the same. In a normal Safari tab the browser may keep that top swipe for itself, so use Add to Home Screen or tap.
- Control Center has three pages (Favorites, Media, Connectivity). Use the dots on the right edge or swipe up and down.
- Long press: the connectivity cluster and Now Playing tile open their full pages; Dark Mode, Sound, flashlight and timer open option sheets; Display opens the brightness panel.
- Connectivity switches are demo state saved on the device (Airplane Mode really hides the signal and Wi-Fi icons). Now Playing plays a short generated tune; AirPlay opens sound.sim.

