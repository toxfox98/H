# Riftbound Atlas Mobile v0.9 — GitHub Mobile Package

This package is intentionally reduced to **5 uploadable files**.

## Upload these 3 root files
1. `index.html`
2. `package.json`
3. `README.md`

## Then create this folder path in GitHub and upload the 2 workflow files
`.github/workflows/`

Upload:
- `build-android.yml`
- `deploy-pages.yml`

You do NOT need to upload `src`, `public`, `scripts`, `data`, `android`, `node_modules`, or any other folders.

## Build the APK from a phone
1. Open the repository's **Actions** tab.
2. Select **Build Android APK**.
3. Tap **Run workflow**.
4. Wait for the green check.
5. Open the completed workflow run.
6. Under **Artifacts**, select `Riftbound-Atlas-Android`.
7. Download the artifact ZIP and extract the APK.
8. Install `Riftbound-Atlas-Android.apk` on Android.

## Web version
The `Deploy Riftbound Atlas Web App` workflow runs when you push to `main`, or you can run it manually from Actions.

## Important
The APK is a debug build for testing with friends. It does not require Node.js, Git, Android Studio, or the source project on the phone running the APK.

Card data is loaded from the public Riftbound card-data release at runtime, so the package stays small and does not require a giant `cards.json` upload.
