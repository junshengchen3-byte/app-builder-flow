---
name: app-builder-flow
description: Use when guiding an app idea or existing app through product definition, UI direction, implementation planning, testing, and release preparation. Do not use for ordinary article writing, README-only work, or GitHub-only setup unless the request is part of app product/release planning.
metadata:
  short-description: Turn an app idea into an MVP and release plan
---

# App Builder Flow

Use this skill to help a person turn an app idea into a usable, testable, releasable product. Do not turn the user's app into a fixed template. The app type, platform, UI style, data model, backend needs, and release path must come from the user's goals and constraints.

Do not use this skill for ordinary article drafting, article rewriting, document polishing, repository housekeeping, or GitHub publishing tasks when the user is not asking to define, build, test, or release an app. Handle those requests directly or route to a more specific skill.

## Operating Rules

- Start by clarifying product intent before implementation: target user, core job, must-have features, out-of-scope items, monetization, platforms, and release target.
- Prefer a small releasable MVP over a broad first version.
- Do not introduce login, cloud sync, payments, AI, or a backend unless the product need requires it.
- Separate decisions from execution. Produce a decision-complete plan before making broad implementation changes.
- During implementation, preserve existing project behavior unless the user explicitly changes the product direction.
- Surface blockers immediately with the reason and the concrete way to resolve them.

## Interaction Protocol

- Ask in small batches. Start with the minimum questions needed to identify the product, user, core job, platform, and MVP must-haves.
- Prefer concrete choices when a decision affects implementation: platform, backend, login, monetization, release target, and visual direction.
- After each stage, summarize the locked decisions and open blockers before moving on.
- If the user says "next" or asks to continue, advance to the next unblocked stage and state any user-owned dependency.
- If the user asks to build immediately, first produce a compact decision-complete implementation plan unless the project is already fully specified.

## Stage Routing

Read only the reference needed for the current stage:

- For first-time product discovery, read `references/discovery-questions.md`.
- For sequencing work from idea to release, read `references/stage-gates.md`.
- For required deliverables at each stage, read `references/implementation-output.md`.
- For platform launch, permissions, screenshots, privacy, or store submission, read `references/release-checklists.md`.

## Default Flow

1. Discover the product: what app, who uses it, what problem it solves, what is not included.
2. Design the MVP: user paths, screens, core functions, data, permissions, failure states.
3. Choose the technical route: native, cross-platform, web/PWA, backend, database, deployment.
4. Design UI direction: references, brand, density, components, interaction rules, responsive targets.
5. Implement iteratively: build the smallest vertical slice first, then expand by tested workflows.
6. Add backend only when needed: accounts, sync, payments, AI, collaboration, admin, analytics, or remote content.
7. Verify: automated tests, manual flows, device/browser coverage, permission denial, persistence, and failure handling.
8. Prepare release: app identity, icons, screenshots, privacy disclosures, signing, builds, submission, and review notes.

## Required Plan Shape

When planning a new app, include:

- Summary
- Core users and use cases
- MVP scope and explicit non-goals
- Screens and interaction flow
- Data model and storage choice
- Backend/API decision
- Failure handling
- Testing and acceptance criteria
- Release path and known blockers
- Default decisions

Keep examples generic. Do not copy product-specific details from prior apps unless the user asks to build that exact product.

## Pressure Test Standard

Before considering this skill ready, test it against unrelated requests:

- iOS app planning, such as a teleprompter, habit tracker, booking app, or local utility.
- Web or SaaS product planning, such as an admin dashboard, customer form, internal tool, or content workflow.
- Article or documentation requests, such as rewriting a post, creating a README, or preparing GitHub setup steps.

The first two categories should produce product-specific app planning. The third category should not trigger the full App Builder flow unless the user explicitly connects it to app product or release planning.
