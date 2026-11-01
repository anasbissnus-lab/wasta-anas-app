# WASTA ANAS Android App

## GitHub upload
Upload the contents of this folder to the root of your GitHub repository (not the outer ZIP folder):
- `package.json`
- `capacitor.config.json`
- `www/index.html`
- `.github/workflows/android-apk.yml`

Then commit to the `main` branch. GitHub Actions will build a debug APK.

## Download APK
In GitHub, open the repository > Actions > Build Wasta Anas APK > latest successful run > Artifacts > `wasta-anas-debug-apk`.

## Supabase
Open the app, enter your Supabase Project URL and Publishable/anon key. Never put a `service_role` key in the app.
The app expects tables `profiles`, `projects`, `expenses`, and `staff`. Set secure Row Level Security policies in Supabase before using real business data. A profile row must already exist for each Auth user; set the owner's role to `admin` securely in Supabase SQL/editor.
