# Haven · Property management

A responsive property management demo built with React and Vite. It includes two role experiences (owner/manager and tenant), local-storage login and signup, property management, rent activity, and a guided presentation flow.

## Run locally

```sh
npm install
npm run dev
```

Use the **Owner / manager** or **Tenant** role and the demo account `demo@haven.co` / `haven123`. New accounts can also be created. Demo accounts and changes are stored in this browser's local storage; clearing site data resets the demo. This is a classroom prototype, not a production authentication or payments service.

## Implementation

- Vite + React, with responsive CSS Grid and Flexbox layouts.
- Owner module: portfolio metrics, property list/search/filter, add-property dialog, rent activity, and payment overview.
- Tenant module: personal home and activity, with a simulated rent-payment action.
- Authentication: signup/sign-in and demo access backed by `haven_users` and `haven_session` local-storage keys.
- Persistence: properties and payment activity use `haven_properties` and `haven_tx`.

## Deployment (Vercel or Git-backed host)

Build command: `npm run build` · Output directory: `dist` · Install command: `npm install` · Framework preset: Vite. Import this repository in Vercel or connect the Git provider; no environment variables are needed. Vite's SPA fallback is handled by the host's Vite preset. For a static GitHub Pages subpath, configure Vite's `base` to match the repository path first.

## Rubric mapping and demo plan

See [Review guide](docs/REVIEW-GUIDE.md) and [LinkedIn article draft](docs/LINKEDIN-ARTICLE.md). The guide maps all Review 1 and Review 2 rubric lines to the implemented screens and offers a short walkthrough and contribution template. Replace the contribution placeholders with the actual team members and their work before presenting.
