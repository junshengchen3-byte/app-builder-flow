# Stage Gates

Use stage gates to prevent coding before the product is clear and to prevent release before the app is verified.

## 1. Product Gate

Required before detailed planning:

- One-sentence product positioning.
- Primary user and core scenario.
- MVP must-haves and non-goals.
- Target platform and release target.

Blocker handling: if the user cannot choose a platform, recommend the route with the smallest credible path to release.

## 2. Flow Gate

Required before UI design:

- Main user path from opening the app to finishing the core job.
- Screen list and navigation model.
- Required permissions and when they are requested.
- Empty, loading, error, and denied-permission states.

Blocker handling: if the main path is unclear, design one default happy path and ask the user to confirm.

## 3. Technical Gate

Required before implementation:

- Chosen client stack.
- Storage model: local, hosted backend, third-party backend, or hybrid.
- Backend decision with reason.
- External services and account requirements.
- Build/test commands.

Default: no backend unless the app requires shared state, accounts, payments, AI, admin, remote content, or analytics.

## 4. UI Gate

Required before building screens:

- Visual direction or reference.
- Core components and layout density.
- Key interaction rules.
- Responsive targets.
- App icon or brand direction if applicable.

Blocker handling: if no style reference exists, produce two to three contrasting directions and recommend one.

## 5. Implementation Gate

Required during build:

- Implement one vertical slice first.
- Add tests for core behavior and risky state transitions.
- Run build/test after meaningful changes.
- Keep a known blockers list.

Blocker handling: state whether the blocker is product, technical, account, device, or release-related, then give the resolution path.

## 6. Release Gate

Required before submission:

- Final app name and identifier.
- Icon and launch assets.
- Permission strings and privacy disclosures.
- Store screenshots and description.
- Signing/account access.
- Device/browser verification for critical paths.

Blocker handling: do not claim release readiness until account, signing, and real-device or production-environment checks are complete.
