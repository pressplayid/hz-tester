# Press Play Hz Tester App

Check whether your mouse really reaches **1K, 2K, 4K or 8K** polling. Windows 10/11, nothing to install, runs fully offline.

This is a private archive of release builds. The public download lives on pressplayid.com.

## How to use

1. Double-click `PressPlay Hz Tester App.exe`.
2. Pick the polling rate your mouse is set to (in your mouse software).
3. Press **Start**, then move your mouse in big, fast circles for 10 seconds.
4. Read the result. **Show details** has the charts; **Export CSV** saves every report.

## Tips for an accurate result

- Plug the mouse or receiver straight into a USB port on the back of the PC, not a hub.
- For 4K/8K, use the high-polling receiver that came with the mouse.
- Move fast: slow movement sends fewer reports.

## "Windows protected your PC"

The app isn't code-signed yet, so Windows may show this on first run. Click **More info**, then **Run anyway**.

## How it measures

Windows Raw Input on a dedicated high-priority thread, every report timestamped with the Windows high-resolution timer (QueryPerformanceCounter, 100 ns). The verdict uses rate stability (100 ms windows reaching ≥95% of the rate); missed reports are expected slots minus reports received. Software-injected input is ignored. The USB link check reads bus speed and the mouse endpoint's polling interval from Windows.

## Requirements

Windows 10 (1903+) or Windows 11, 64-bit.

---

© 2026 Press Play · [pressplayid.com](https://pressplayid.com) · Fonts: Epilogue and Inter, SIL Open Font License 1.1.
