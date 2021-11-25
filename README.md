# Charles Proxy iOS setup guide

## Purpose of this repo

This repo explains how to setup Charles Proxy on your Mac and use it as a proxy for your iOS device.

## Basic installation steps

1. Download and install [Charles Proxy](https://www.charlesproxy.com/) on your Mac.
2. Open Charles Proxy on your Mac.
3. Make sure that your Mac and your iOS device are connected on the same local network
4. On your iOS device, go to Settings > Wi-Fi
5. Click on the info icon at the right of your currently connected network
6. In the HTTP Proxy section, go to Configure proxy > Manual
7. Fill the server field with the local IP address of your Mac (generally something like 192.168.x.y).
8. Fill the port field with 8888.
9. Open Safari on your iOS device and go to any URL. You should see a popup from Charles Proxy on your Mac asking you to allow your iOS device to use the Proxy.
10. Click on "Allow".

## HTTPS setup

Do the following setps if you want to debug HTTPS requests.

1. On your iOS device, open Safari and enter [this url](https://chls.pro/ssl).
2. You should see an alert asking you if you want to install the certificate. Install it.
3. Go to Settings > General > Profiles.
4. Find the installed profile. Click on it and enable it.
5. Go to Settings > General > About > Certificate Trust Testings and enable the installed profile.
