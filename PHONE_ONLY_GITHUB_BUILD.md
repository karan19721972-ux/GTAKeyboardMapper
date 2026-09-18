# Phone-only build instructions

1. Create a GitHub repository, e.g. `GTAKeyboardMapper`.
2. Upload/extract this project's files into the repository root.
3. Commit to `main` (or `master`).
4. Open the repository's **Actions** tab.
5. Select **Build Android APK**.
6. Press **Run workflow**.
7. Wait for the green check.
8. Open the completed workflow run and download the artifact named `GTAKeyboardMapper-debug`.
9. Extract the artifact ZIP and install the APK on the phone.

If GitHub does not show the workflow, check that `.github/workflows/android.yml` is present in the repository and refresh the Actions page.

The build is a debug APK for testing. Android may require permission to install apps from the browser/file manager you use.
