# PrinterMonitor Support

Need help with PrinterMonitor? Email me and I'll get back to you as soon as I can.

**Email: [vasapol.aurean@gmail.com](mailto:vasapol.aurean@gmail.com)**

## When you write, please include

- Your device and system version (for example iPhone 16, iOS 27, or Mac, macOS 26)
- The app version (shown in the App Store)
- Your printer's firmware and mode, if you know it (RepRapFirmware 3 standalone, SBC, or older RepRapFirmware 1/2)
- What you did, what you expected, and what happened instead
- A screenshot, if it helps

Please do not send printer passwords by email.

## Frequently asked questions

### The app can't connect to my printer
- Make sure your phone or Mac is on the **same network** as the printer.
- Enter the printer's IP address (for example 192.168.0.60) or hostname, and the port (usually 80).
- Open the address in a web browser on the same device. If the printer's own web page doesn't load, the app can't reach it either.
- If your printer has a password, enter it in the printer settings.
- Allow **Local Network** access for PrinterMonitor when iOS asks. You can change this later in Settings → Privacy & Security → Local Network.
- Use **Test Connection** in the printer settings to see the detected firmware or the error.

### Which printers are supported?
PrinterMonitor works with printers running RepRapFirmware: version 3 in standalone and SBC mode, and older versions 1 and 2. The mode is detected automatically.

### My printer shows as offline
Check the printer is powered on and on the network, then open the printer page again. Small controller boards can only handle a few connections at once, so close other apps or browser tabs that are connected to the same printer.

### Fan speed goes back to its old value
A fan that is controlled by a heater (thermostatic) takes control back. In the Control tab, turn off the **auto (heater-controlled)** switch for that fan first, then set the speed. During a print, fan commands in the G-code file can also override your setting.

### How do I add a camera?
Edit the printer and enter the camera URL. MJPEG streams (for example `http://<printer>:8080/?action=stream`) and snapshot image URLs are supported. Other formats such as RTSP or WebRTC are not supported.

### I don't see file thumbnails
Thumbnails only appear if your slicer embeds them in the G-code file (the printer firmware must also support them). The toolpath preview works without thumbnails.

### Where is my data stored?
Printer details and settings stay on your device, and printer passwords are stored in the Keychain. Nothing is sent to the developer. See the Privacy Policy for details.

### I have a feature request
Please email it. Ideas are welcome.

---

*PrinterMonitor is an independent app and is not affiliated with or endorsed by Duet3D Ltd. or the RepRapFirmware project.*
