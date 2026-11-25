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
- Owner module: portfolio metrics, property list/search/filter, add-property dialog, tenant view, rent activity, lease-renewal review, and owner–tenant messaging.
- Tenant module: personal home and payment history, lease-renewal requests, messaging, and a simulated rent-payment action.
- Authentication: signup/sign-in and demo access backed by `haven_users` and `haven_session` local-storage keys.
- Persistence: properties, payment activity, lease records, and messages are stored in this browser's local storage.

## Deployment

GitHub repository: [krishnareddy2318/haven-property-management](https://github.com/krishnareddy2318/haven-property-management)  
Production site: [haven-property-management.vercel.app](https://haven-property-management.vercel.app)

Build command: `npm run build` · Output directory: `dist` · Install command: `npm install` · Framework preset: Vite. The Vercel project is connected to the GitHub repository's `main` branch. No environment variables are required. For GitHub Pages under a repository subpath, configure Vite's `base` first.

## Rubric mapping and demo plan

See the [Review guide](docs/REVIEW-GUIDE.md) and the [published LinkedIn article](https://www.linkedin.com/pulse/making-property-management-feel-more-human-our-haven-project-reddy-jj9bc/). The guide maps each Review 1 and Review 2 rubric line to the implemented screens and provides a short walkthrough. Confirm the team crew's specific task contributions before presenting.
