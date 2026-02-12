CUSTOM COMMUNICATIONS - CRV DIGITAL VFO SUITE
Beta Test Version 1.0

Thank you for testing the CRV Digital VFO firmware and configuration suite. This package contains everything you need to flash your hardware and customize your radio settings.

---
FILE LIST:
---
1. flasher.html      - The firmware update tool.
2. configurator.html - The radio settings and frequency database tool.
3. manifest.json     - Support file for the flasher.
4. firmware.bin      - The CRV system firmware.

---
SETUP INSTRUCTIONS (CRITICAL):
---
Browser Support: You MUST use a Chromium-based browser (Google Chrome, Microsoft Edge, or Brave). Firefox and Safari DO NOT support the "Web Serial" technology required to talk to your radio.

Local Server Requirement: For security reasons, browsers block these tools if you simply double-click the HTML files from your folder. To use them, you must host them on a local web server. 
- Recommendation: Use the "Web Server for Chrome" extension or upload the contents of this ZIP to your personal web hosting.
- Check: Once loaded, the "Local Manifest" indicator should turn GREEN.

---
HOW TO FLASH:
---
1. Connect your CRV hardware to your computer via USB.
2. Open flasher.html through your web server.
3. If your board does not auto-detect, hold the BOOT button while plugging in the USB or while clicking "Flash."
4. Select the correct COM port (usually labeled CH340 or CP210x) in the pop-up window.
5. Wait for the progress bar to reach 100%.

---
HOW TO CONFIGURE:
---
1. Once flashed, use the link at the top of the page to switch to the "Radio Configurator."
2. Click "Connect" to open the serial link to your radio.
3. Use the built-in database and formula tools to set your VFO parameters.
4. Click "Save to Radio" to commit your changes.

---
TROUBLESHOOTING:
---
- RED STATUS DOT: The browser cannot see the manifest.json file. Ensure you are running through a web server and not just opening the file directly from your hard drive.
- FAILED TO OPEN PORT: Ensure the Arduino IDE Serial Monitor or any other terminal programs are CLOSED. Only one program can use the radio's port at a time.
- PERMISSIONS (Linux Users): Ensure your user is in the 'dialout' group and that the 'brltty' service is disabled/removed.

For technical support or to report bugs, please contact Custom Communications.
