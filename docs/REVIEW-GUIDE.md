# Project review guide — Haven

## Business system and modules

Haven supports property owners/managers and renters in the same rental workflow. The selected role is stored with the session and controls the dashboard experience.

| Module | Responsibilities | Demonstration |
|---|---|---|
| Admin / owner | Review portfolio and rent metrics; search/filter properties; add a listing; review tenants and rent activity; manage lease renewals; exchange messages with tenants. | Select **Owner / manager**, sign in with the demo account, add a listing, open **Leases** and approve a renewal, then send a message. |
| User / tenant | See their home, lease, and personal payment history; request a lease renewal; message the owner; record a sample rent payment. | Sign out, select **Tenant**, use the demo account, request renewal in **Leases**, send a message, and record a payment in **Payments**. |

## Review 1 rubric

1. **Business system and module identification:** owner and tenant roles and responsibilities are listed above.
2. **UI template and layout:** responsive CSS Grid cards and two-column dashboard; Flexbox navigation, rows, and toolbars; mobile navigation drawer.
3. **Login and signup using local storage:** account creation and session persistence use `haven_users` and `haven_session`. Demo credentials: `demo@haven.co` / `haven123`. This classroom-only approach stores demo passwords in browser storage; production authentication requires a secure backend.
4. **Project demonstration and explanation:** follow the 3-minute walkthrough below. Explain role-based workflows, local persistence, property/payment activity, lease renewals, and owner–tenant messages.
5. **LinkedIn article with DTI concepts and review:** use the editable draft in [LINKEDIN-ARTICLE.md](LINKEDIN-ARTICLE.md). Replace bracketed details and insert the actual review outcome before publishing.
6. **Git deployment:** the project is published at [krishnareddy2318/haven-property-management](https://github.com/krishnareddy2318/haven-property-management). The production app is live at [haven-property-management.vercel.app](https://haven-property-management.vercel.app). Deployment settings are in the README.

## Review 2 rubric

1. **React Vite implementation:** `package.json`, `vite.config.js`, `index.html`, and `src/` implement the React + Vite app.
2. **Login and signup with local storage:** same authentication flow as Review 1; signup, logout, and sign-in preserve the session across reloads.
3. **Admin/user modules, UI, functionality:** role experiences, property creation and filtering, role-filtered payment history, lease renewal requests, browser-local owner–tenant messages, responsive UI, and feedback toasts are implemented.
4. **Vercel/Git deployment:** the Vercel production deployment is live at [haven-property-management.vercel.app](https://haven-property-management.vercel.app), built from the GitHub repository's `main` branch with `npm install`, `npm run build`, and output `dist`.
5. **Team coordination and individual contribution:** the known project-coordination contribution is recorded below. If this is a group submission, add each remaining member and their verified work before presenting; do not guess contributions.

| Team member | Individual contribution | Evidence / file or screen |
|---|---|---|
| Krishna Reddy — project coordination | Defined the project brief and rubric scope; authorized the public GitHub repository and Vercel deployment; reviewed the owner and tenant workflows. | Project brief; [public repository](https://github.com/krishnareddy2318/haven-property-management); [live demo](https://haven-property-management.vercel.app) |

## Suggested 3-minute presentation

1. **0:00–0:25 — Problem and users:** describe fragmented landlord workflows and identify owners/managers and tenants.
2. **0:25–0:55 — Sign-in:** show the role selector and local-storage demo sign-in; explain that signup creates a local demo account.
3. **0:55–1:40 — Owner:** present portfolio metrics, search/filter properties, add a sample property, review rent activity, and mark a lease renewal.
4. **1:40–2:15 — Tenant:** sign out, enter tenant mode, view the home and personal payments, request renewal, exchange a message, and record a sample payment.
5. **2:15–2:45 — Design and technology:** point out Grid/Flex responsive layout, React components/state, and browser persistence for properties, leases, messages, and payments.
6. **2:45–3:00 — Review and deployment:** share the real hosted URL and actual contribution split; explain one improvement the team would make next.

## Scope and production follow-up

The property, lease, message, and payment records are browser-local demo data. Lease renewal actions update local status; messages stay in the current browser; rent payment is simulated. Replace local-only storage with authenticated APIs and server-side authorization, and connect a payment provider before handling real tenants or money. Lease documents and maintenance requests are future enhancements.
