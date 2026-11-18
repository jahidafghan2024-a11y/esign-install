# ESign Install

Direct over-the-air (OTA) install page for **ESign Reborn 6.2.0** (`dev.esignreborn.app`), signed with the free **Chengdu Railway Bureau** enterprise certificate (valid to Oct 2, 2027).

Live site (GitHub Pages): https://jahidafghan2024-a11y.github.io/esign-install/

## Install

1. Open the live site in Safari on your iPhone.
2. Tap **Install ESign** and confirm the install pop-up.
3. Go to **Settings > General > VPN & Device Management**, tap the **Chengdu Railway Bureau** certificate and tap **Trust**.
4. Open ESign. To sign other apps with the same certificate, import `Chengdu_Railway_Bureau.p12` and `Chengdu_Railway_Bureau.mobileprovision` from this repo into ESign (the password is shown on the install page).

## Files

- `index.html` — the install page (also works as a Telegram Mini App)
- `manifest.plist` — iOS OTA manifest, points at `esign-signed.ipa`
- `esign-signed.ipa` — ESign Reborn 6.2.0, already signed
- `Chengdu_Railway_Bureau.p12` / `Chengdu_Railway_Bureau.mobileprovision` — the free certificate files

## When the certificate changes

Re-sign the ESign IPA with the new certificate, replace `esign-signed.ipa` and the two certificate files, and update the name/expiry shown on the install page. The manifest stays the same unless the app version changes.
