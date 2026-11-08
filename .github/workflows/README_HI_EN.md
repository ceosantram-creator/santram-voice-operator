# SANTRAM 9999999999999X — phone-only cloud APK build

## Files
- Android source project is in this ZIP under `SANTRAM_9999999999999X_Android_MVP/`.
- `GITHUB_ACTIONS_WORKFLOW.txt` is the workflow text to paste into GitHub.
- This project is an MVP source package, not a compiled APK.

## Build from your Android phone using GitHub Actions
1. Download this ZIP to your phone.
2. Sign in or create an account at https://github.com using Chrome.
3. In GitHub, create a new **private** repository named `santram-voice-operator`. Do not initialize it with a README, license or .gitignore.
4. In the new empty repository, choose **Add file → Upload files** and upload this ZIP file itself. Rename it `santram-source.zip` if needed, then commit it to `main`. Do not extract it before uploading.
5. In the repository choose **Add file → Create new file**.
6. In the filename field enter exactly `.github/workflows/build.yml` (GitHub creates the folders from the path).
7. Open `GITHUB_ACTIONS_WORKFLOW.txt` from this downloaded ZIP using your phone's text viewer, copy its entire content, and paste it into the GitHub editor.
8. Commit the new file to `main`.
9. Open the repository's **Actions** tab. Select **Build SANTRAM Android APK**. Tap **Run workflow** if it has not started automatically.
10. Wait for a green successful run. Open the completed run, scroll to **Artifacts**, and download `SANTRAM-9999999999999X-debug-apk`.
11. Extract the downloaded artifact ZIP. Inside it, find `app-debug.apk`.
12. Tap the APK to install. If Android asks, allow your browser or file manager to install unknown apps for this installation. After install, turn that permission back off.
13. Open SANTRAM Voice Operator, grant microphone permission, choose Hindi or English, and tap **TAP TO SPEAK**.

## If the build fails
- Open the failed workflow run and expand the red failed step.
- Copy the first actual error message (not the entire log) and share it here.
- Do not share passwords, GitHub recovery codes, access tokens, or API keys.

## What this V1 does / does not do
- Does: tap-to-speak speech recognition (Hindi India / English India), local text-to-speech, and launching a small allowlist of installed apps.
- Does not: keep listening in the background, send recognized speech automatically into ChatGPT, or remotely control every Android app.
- Open-ended AI questions are handed off by opening ChatGPT. No OpenAI API key is required for the local MVP features.
- The APK produced is a debug/test APK. It is not Play Store release-signed.

## Privacy and security
- Keep the repository private because it contains your source code.
- The app requests microphone permission only.
- No OpenAI API key is present in the source or APK.
- Disable "install unknown apps" permission again after installing.
