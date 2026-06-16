# Puretip One — OTA update channel

Public distribution channel for the **Puretip One** station tablet app (compiled APK +
update manifest). The application **source is private**; this repo holds only the signed,
shipping artifacts so tablets can self-update over HTTPS.

- `latest.json` — the update manifest the app polls.
- Releases — each `PuretipOne-vX.YY.apk` (signed with the IonField/Augeas release key).

Tablets read `latest.json` and, if a newer `versionCode` is published (and the tablet is in
`targets`, or `targets` is omitted = all), download and install it. See the integration docs
in the main project for batch vs individual roll-out.

© IonField Systems · built by Augeas Technologies.
