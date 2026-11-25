# Project review guide — Haven

## Business system and modules

Haven supports property owners/managers and renters in the same rental workflow. The selected role is stored with the session and controls the dashboard experience.

| Module | Responsibilities | Demonstration |
|---|---|---|
| Admin / owner | Review portfolio and rent metrics; search/filter properties; add a listing; see tenants and payment activity; open navigation to leases, settings, and messages. | Select **Owner / manager**, sign in with the demo account, add a listing, then filter to vacant homes. |
| User / tenant | See their home and rent activity, review the payment overview, and record a sample rent payment. | Sign out, select **Tenant**, use the demo account and click **Record rent payment**. |

## Review 1 rubric

1. **Business system and module identification:** owner and tenant roles and responsibilities are listed above.
2. **UI template and layout:** responsive CSS Grid cards and two-column dashboard; Flexbox navigation, rows, and toolbars; mobile navigation drawer.
3. **Login and signup using local storage:** account creation and session persistence use `haven_users` and `haven_session`. Demo credentials: `demo@haven.co` / `haven123`. This classroom-only approach stores demo passwords in browser storage; production authentication requires a secure backend.
4. **Project demonstration and explanation:** follow the 3-minute walkthrough below. Explain role-based workflows, local persistence, and the property/payment interaction.
5. **LinkedIn article with DTI concepts and review:** use the editable draft in [LINKEDIN-ARTICLE.md](LINKEDIN-ARTICLE.md). Replace bracketed details and insert the actual review outcome before publishing.
6. **Git deployment:** the project is published at [krishnareddy2318/haven-property-management](https://github.com/krishnareddy2318/haven-property-management). The production app is live at [haven-property-management.vercel.app](https://haven-property-management.vercel.app). Deployment settings are in the README.

## Review 2 rubric

1. **React Vite implementation:** `package.json`, `vite.config.js`, `index.html`, and `src/` implement the React + Vite app.
2. **Login and signup with local storage:** same authentication flow as Review 1; signup, logout, and sign-in preserve the session across reloads.
3. **Admin/user modules, UI, functionality:** role experiences, property creation and filtering, sample payment activity, responsive UI, and feedback toasts are implemented.
4. **Vercel/Git deployment:** the Vercel production deployment is live at [haven-property-management.vercel.app](https://haven-property-management.vercel.app), built from the GitHub repository's `main` branch with `npm install`, `npm run build`, and output `dist`.
5. **Team coordination and individual contribution:** use the contribution table below during the presentation. Enter each member's real name and work; do not claim contributions that were not made.

| Team member | Individual contribution | Evidence / file or screen |
|---|---|---|
| [Name 1] | [e.g. owner module and property workflow] | [Files / demo] |
| [Name 2] | [e.g. tenant module and local storage] | [Files / demo] |
| [Name 3] | [e.g. responsive UI, documentation and deployment] | [Files / demo] |

## Suggested 3-minute presentation

1. **0:00–0:25 — Problem and users:** describe fragmented landlord workflows and identify owners/managers and tenants.
2. **0:25–0:55 — Sign-in:** show the role selector and local-storage demo sign-in; explain that signup creates a local demo account.
3. **0:55–1:40 — Owner:** present portfolio metrics, search/filter properties, add a sample property, and point out recent rent activity.
4. **1:40–2:15 — Tenant:** sign out, enter tenant mode, view the home and record a sample payment.
5. **2:15–2:45 — Design and technology:** point out Grid/Flex responsive layout, React components/state, and browser persistence.
6. **2:45–3:00 — Review and deployment:** share the real hosted URL and actual contribution split; explain one improvement the team would make next.

## Scope and production follow-up

The property records and payments are sample data, and the tenant payment button only adds a local activity record. Sidebar areas such as messages and leases are navigation placeholders. Replace local-only storage and simulated payments with authenticated APIs, server-side authorization, validated persistence, and a payment provider before handling real tenants or money.
