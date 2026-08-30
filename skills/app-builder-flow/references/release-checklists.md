# Release Checklists

Use the checklist matching the target platform. Do not mark account, signing, payment, or store submission work complete unless it was actually verified.

## iOS / iPadOS

- App name, bundle identifier, version, and build number are set.
- App icon, launch assets, and required image sets are included.
- `Info.plist` permission strings match actual usage.
- `PrivacyInfo.xcprivacy` is present when required.
- iPhone and iPad layouts are verified if both device families are supported.
- Simulator tests pass, but camera, microphone, photos, notifications, purchases, and background behavior require real-device checks.
- Apple Developer Team is configured.
- Archive succeeds.
- TestFlight upload succeeds.
- Review notes explain permissions, login requirements, and demo access if needed.

## Android

- App name, package name, version name, and version code are set.
- Launcher icons and adaptive icon assets are included.
- Runtime permissions match actual usage.
- Privacy policy and Data safety answers match the app's behavior.
- Phone and tablet layouts are checked if supported.
- Signed release build is generated with a managed keystore.
- Internal testing track is used before production.

## Web / PWA

- Production URL, app name, favicon, social preview, and manifest are set.
- Build command and deployment target are verified.
- Environment variables are documented and configured.
- Auth, payments, analytics, and storage rules are verified in production mode.
- Responsive layouts are checked on mobile and desktop.
- Error pages, loading states, and empty states are verified.
- Privacy policy and terms are linked when user data is collected.

## Backend Or Cloud Services

- Production database and storage are separate from development.
- Secrets are not committed.
- Migrations are repeatable.
- Backups or export path exist for important user data.
- API failures have user-facing handling.
- Rate limits, quotas, and billing risks are documented.
- Logs do not expose private user content.
