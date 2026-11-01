12C CLASSIC — OFFLINE PWA

WHAT'S INCLUDED
- index.html: the calculator app (no external scripts, fonts, APIs or CDN dependencies)
- manifest.webmanifest + sw.js: installable Progressive Web App and offline cache
- icon-192.png + icon-512.png: home-screen icons

TRY IT IMMEDIATELY ON ANDROID
1. Download and extract the ZIP on the phone.
2. In Files, tap index.html and choose Chrome (or use Open with Chrome).
3. Try the keys. The app itself works without a network connection.
4. Tap HAPTIC ✓ to enable or HAPTIC OFF to disable the vibration pulse.

INSTALL IT AS A HOME-SCREEN APP (RECOMMENDED)
A PWA must be served from HTTPS (or localhost) for installation and service-worker offline caching.
1. Create a GitHub repository and upload the contents of this folder to the repository root.
2. In the repository, open Settings → Pages. Under Build and deployment, choose Deploy from a branch, select the main branch and /(root), then Save.
3. Wait for GitHub Pages to publish the site, then open the published HTTPS URL in Chrome on Android.
4. Open Chrome's ⋮ menu and choose Install app (or Add to Home screen, depending on Chrome version).
5. Launch the new 12C Classic icon. After its first load, the app shell is cached for offline use.

HAPTICS
The app requests a short 9 ms vibration pulse for each tap on a calculator key using the browser Vibration API. Android Chrome generally supports this; the phone's system vibration setting controls its intensity. If a key does not vibrate, enable system touch/vibration feedback and make sure HAPTIC is on in the app. Actual vibration must be checked on the target phone.

FUNCTIONAL SCOPE
Implemented: RPN entry and four-level stack operations; basic arithmetic; percentages; sign change and scientific exponent entry; reciprocal and powers; 20 data registers; core TVM calculations (n, i, PV, PMT, FV); begin/end payment mode; NPV and IRR cash-flow entry; a basic amortization routine; date addition/day-count; simple interest basis selection; and a simple statistics accumulator. Keystroke programming and some specialist bond/depreciation routines are not complete. Always independently verify important financial calculations.

The calculator's key layout and color-coded f/g convention are inspired by the classic HP 12C. This is an independent companion, not an official HP application and not affiliated with Hewlett-Packard.


VISUAL UPDATE
- The calculator now opens in landscape orientation (PWA manifest orientation).
- The face is scaled as a single landscape unit to match the proportions of the supplied reference.
- The top panel, LCD position, key spacing, and legends have been adjusted toward the reference photograph.
- On browsers that cannot lock orientation, portrait mode displays a rotate-phone prompt.
- Haptics use the device vibration API where the browser and hardware support it.

LIMITATION
This remains an independent 12C-style companion, not an official HP product or a verified
bit-for-bit firmware emulator. Some advanced original routines and program-mode features
remain approximations or are not implemented; see the in-app guide/source.


VISUAL UPDATE 3
- Fixed 600x375 stage (measured from the reference image) scaled to any screen: exact key pitch, row spacing, orange/blue legends, BOND, DEPRECIATION and CLEAR brackets, corrected legends (ΔDYS, x̄ w, n!, x̂ r, ŷ r, x≷y, ←).

VISUAL UPDATE 2
- The ten key columns now use narrower key faces and wider, more realistic gaps.
- Key height and row spacing now follow the reference photograph more closely.
- The ENTER key lettering is stacked vertically.
- Orange function labels and cyan secondary labels have been enlarged and recolored.
- Added the missing DATE and MEM legends and the CLEAR bracket.
- Corrected the duplicate haptic-toggle element and refreshed the offline cache version.

For the largest usable view, install the PWA from its HTTPS address and launch it
from the home-screen icon. Opening index.html inside a file viewer or browser tab
leaves browser/system bars visible and reduces the available calculator area.


ENGINE UPDATE (v4)
- Corrected f/g functions, f+digit decimals, AMORT, INT, SL/SOYD/DB, DATE/DYS, statistics (x-bar, s, x-hat, y-hat, x-bar w, Sigma-), n!, sqrt, e^x, LN, FRAC, INTG, backspace, EEX entry, n rounded up.
- Still not included: keystroke programming, PRICE, YTM, x<=y, x=0, GTO.


FINAL (v5)
- Keystroke programming (f P/R, R/S, SST, g BST, g GTO nn, g x<=y, g x=0), PRICE and YTM added.
- APK: upload this folder (including .github) to a GitHub repo; Actions > Build APK > Run workflow; download 12c-classic-apk from the run artifacts and install app-debug.apk (allow unknown sources).


v6: the face now stretches to fill any screen shape (phone or tablet). Text keeps its proportions; keys, rows and the display spread into the extra space.
