Environment

Device: Mac mini (Apple M4)

OS: macOS


Browsers:

Google Chrome Version 145.0.7632.160 (Official Build) (arm64)

Firefox 148.0.2 (aarch64)

Safari Version 26.3.1 (21623.2.7.11.7)

Preconditions
User opens the Waivers page.

Steps to Reproduce

Navigate to https://guest.airtopiapark.com/waivers

Open Waivers & Agreements

Click Waiver → Read Agreement

Observe the agreement text in the modal window.

Actual Result

The agreement text is not visible when the modal opens.
If the user selects the text with the cursor, the text becomes visible.
Expected Result

The agreement text should be visible immediately when the modal opens.

Possible Cause

Font color appears to match or be too close to the background color (likely white text on a white background).

Severity
Medium

Reason: Users cannot read the waiver agreement unless they manually highlight the text.

screenshots
    ├── waiver-text-invisible.png
    └── waiver-text-selected.png
