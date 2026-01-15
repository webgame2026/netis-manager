# Netis Router Manager

A modern, responsive web application for managing Netis routers. This project uses a mobile-first approach and can be installed as a PWA or wrapped into a native app using Capacitor.

## Features
- **Target IP Config**: Specify the router IP (default 192.168.1.1).
- **Dashboard**: Real-time network status monitoring.
- **Internet/WAN**: Configure PPPoE, Static IP, or DHCP connection types and toggle internet access.
- **Wi-Fi Config**: Change SSID and passwords for 2.4GHz and 5GHz bands.
- **Device Management**: View and block connected clients.
- **System Tools**: Reboot and Reset functionality.

## Quick Start
1. Open `index.html` in any modern browser.
2. Confirm the Router IP (default: `192.168.1.1`).
3. Login with default credentials (`admin` / `password`).

## Build for Mobile (Capacitor)
1. Install dependencies:
   ```bash
   npm install @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios
   ```
2. Initialize Capacitor:
   ```bash
   npx cap init
   ```
3. Add platforms:
   ```bash
   npx cap add android
   npx cap add ios
   ```
4. Build your assets (ensure `index.html` is in the `www` folder as configured in `capacitor.config.json`).
5. Sync and Open:
   ```bash
   npx cap sync
   npx cap open android
   ```

## Note
This is a simulation UI. Real-world implementation requires a backend proxy to handle CORS and router-specific binary/HTTP protocols.