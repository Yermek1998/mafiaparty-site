# Mafia Party invitations

Static GitHub Pages site for https://mafiaparty.click.

Publish `main` / root and enable HTTPS. `.nojekyll` keeps `.well-known` files in the published output.

Invite URL: `https://mafiaparty.click/join/?code=123456`.

The page includes a user-initiated `mafiaparty://join?code=123456` fallback. There are no store links until the app has public store listings. Installing the app does not preserve the invitation automatically; reopen the invitation after installation.

## App association

- iOS: team `77729M7R3Y`, bundle `com.jannatfirdays.Mafia`.
- Android: package `com.example.mafia`. The included certificate fingerprint is the local development signing certificate currently also used for release builds in the Android project. Before Google Play publication, add the Play App Signing certificate's SHA-256 fingerprint to `assetlinks.json`.

Both association files must be publicly reachable over HTTPS with no redirect. Only the root domain is registered in the apps; `www` may redirect to it.
