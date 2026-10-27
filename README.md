# Pimatech Sine Bar Calculator

A free, open-source Android calculator for sine bar setups. Calculate total gage-block stack height from an angle, or find an angle from measured stack height. Includes inch/mm units, decimal degrees and degrees/minutes/seconds, a geometry drawing, popup keypad, roller-center length presets and locally saved settings.

## Download

See Releases for the Android APK and matching source archive. Version 1.0.0 is a **development preview**, not a production-signed or Google Play release. Android 8.0 or later. Installs separately from Pimatech Ball Drop. Runs offline without accounts, ads, subscriptions, analytics or Internet permission.

## Source and building

The complete project is in `Pimatech-Sine-Bar-1.0.0-Source.zip`. Extract it and open the `PimatechSineBar` folder in Android Studio. It contains Kotlin/Compose app source, the pure Kotlin calculation engine, Gradle wrapper, tests, operator documentation and validation evidence. JDK 17 and Android SDK 35 are required. See the enclosed README for exact build instructions.

Source is currently preserved as a versioned archive. Private signing keys are excluded.

## Installation

Download the APK from Releases on Android, open it, and allow your browser or Files app to install unknown apps if prompted. Open Pimatech Sine Bar and check a known setup: a 5-inch roller center distance at 30 degrees requires a 2.50000-inch stack.

## Model and limits

h = L × sin(θ); θ = asin(h/L). L is roller center distance, not overall bar length. h is the difference between roller support heights. If the lower roller sits on a base stack, add that height to h for the upper stack. The angle is from the datum, not an included taper angle.

Assumes equal-diameter rollers, flat datum and correct contact. Verify calibrated center distance and measurement capability. Calibration error, wringing, temperature, wear and deflection are not compensated. The app gives total height; it does not select individual blocks. Display resolution is not setup accuracy. Valid mathematical range: 0–90 degrees, with an advisory above 45 degrees.

Build, six math test groups (including 2,000 seeded round trips) and Android lint passed. Developer emulator UI verification was not completed; the owner subsequently installed and accepted this version. Check known setups on your own device before use.

## License

MIT License; see LICENSE. Third-party components retain their own licenses.

Proudly made and released open source by PimaTech.org.
