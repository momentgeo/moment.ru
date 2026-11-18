# MOMENT

GitHub Pages package. Root `index.html` is the app. `download.html` is the public presentation/install page, and `terms.html` is the registration agreement.

After deployment:
- App: `https://<account>.github.io/<repo>/`
- Download/install page: `https://<account>.github.io/<repo>/download.html`
- Agreement: `https://<account>.github.io/<repo>/terms.html`

The app is a web app/PWA, not a native Android APK or iOS IPA. On supported browsers the install prompt appears; on iOS use Safari → Share → Add to Home Screen.

Before public launch, review the agreement, add owner/support contacts and publish a complete privacy policy. Configure Supabase Auth Site URL and Redirect URLs to the deployed origin.
