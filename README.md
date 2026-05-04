# RootRecord — Doc Repo

Educational documentation for **RootRecord**: what it is, how the products fit together, how accounts and the API work, and how developers navigate the workspace.

This repository is meant to **teach**. It is not a substitute for runbooks inside individual code repos (Workers, mobile apps, marketing site), but it connects those pieces into one narrative.

## Who this is for

| Reader | Start here |
|--------|------------|
| New user / customer | [What is RootRecord?](docs/01-introduction/what-is-rootrecord.md) → [Product overview](docs/02-products/overview.md) |
| Someone evaluating the stack | [Platform overview](docs/03-platform/api-overview.md) → [Domains & URLs](docs/03-platform/domains-and-urls.md) |
| Developer joining the org | [Developer onboarding](docs/08-tutorials/developer-onboarding.md) → [Workspace layout](docs/06-development/workspace-layout.md) |
| Solana / web3 curious | [Solana ecosystem](docs/05-solana/solana-ecosystem.md) → [Solana Tools site](docs/05-solana/solana-tools-site.md) |

## Table of contents

### 0. Workspace snapshot

- [Projects in this workspace](docs/00-overview/projects-in-this-workspace.md)

### 1. Introduction

- [What is RootRecord?](docs/01-introduction/what-is-rootrecord.md)
- [Vision & design themes](docs/01-introduction/vision-and-values.md)
- [Glossary](docs/01-introduction/glossary.md)

### 2. Products

- [Product family overview](docs/02-products/overview.md)
- [Business Manager](docs/02-products/business-manager.md)
- [Weather Manager](docs/02-products/weather-manager.md)
- [Token Manager (mobile)](docs/02-products/token-manager.md)
- [Account Hub](docs/02-products/account-hub.md)
- [Marketing website](docs/02-products/marketing-website.md) — [rootrecord.info](https://rootrecord.info)

### 3. Platform

- [API & services overview](docs/03-platform/api-overview.md)
- [Cloudflare Workers](docs/03-platform/cloudflare-workers.md)
- [Data & storage model](docs/03-platform/data-and-storage.md)
- [Domains & URLs](docs/03-platform/domains-and-urls.md)

### 4. Accounts

- [Authentication model](docs/04-accounts/authentication.md)
- [Billing & licensing](docs/04-accounts/billing-and-licensing.md)
- [Privacy & security posture](docs/04-accounts/privacy-and-security.md)

### 5. Solana

- [Solana in the RootRecord stack](docs/05-solana/solana-ecosystem.md)
- [Solana Tools public site](docs/05-solana/solana-tools-site.md)

### 6. Development

- [Workspace layout (Mobile + Web)](docs/06-development/workspace-layout.md)
- [Repos & branches](docs/06-development/repos-and-branches.md)
- [Mobile build & release](docs/06-development/build-and-release-mobile.md)
- [Web Workers & Pages deploy](docs/06-development/build-and-deploy-web.md)

### 7. Operations

- [Crons & background jobs](docs/07-operations/crons-and-background-jobs.md)
- [Observability](docs/07-operations/observability.md)

### 8. Tutorials

- [New user journey](docs/08-tutorials/new-user-journey.md)
- [Developer onboarding](docs/08-tutorials/developer-onboarding.md)
- [Troubleshooting](docs/08-tutorials/troubleshooting.md)

### 9. Reference

- [FAQ](docs/09-reference/faq.md)

### 10. Deep dives

- [Architecture map (Mermaid)](docs/10-deep-dives/architecture-map.md)
- [HTTP request lifecycle](docs/10-deep-dives/request-lifecycle.md)
- [Product comparison table](docs/10-deep-dives/product-comparison-table.md)
- [Weather data pipeline](docs/10-deep-dives/weather-data-pipeline.md)
- [Business data model](docs/10-deep-dives/business-data-model.md)
- [Earn & rewards](docs/10-deep-dives/earn-and-rewards.md)
- [Internal vs external Solana keys](docs/10-deep-dives/internal-vs-external-solana.md)
- [Push notifications (FCM)](docs/10-deep-dives/push-notifications-fcm.md)
- [Stripe flow](docs/10-deep-dives/stripe-flow.md)
- [Capacitor & `file://` routing](docs/10-deep-dives/capacitor-and-file-url.md)
- [D1 migrations primer](docs/10-deep-dives/d1-migrations.md)
- [CORS vs mobile](docs/10-deep-dives/cors-and-mobile.md)
- [Version policy](docs/10-deep-dives/version-policy.md)
- [Feedback & Discord](docs/10-deep-dives/feedback-and-discord.md)

### 11. For educators

- [90-minute workshop outline](docs/11-for-educators/workshop-outline-90min.md)
- [Quiz questions](docs/11-for-educators/quiz-questions.md)

---

Contributions: see [CONTRIBUTING.md](CONTRIBUTING.md).

License: see [LICENSE](LICENSE).

## Publish to GitHub (Doc-Repo)

This folder is a git repo on branch **`main`**. GitHub CLI was installed, but **no `gh` session** is configured in this environment, so the remote was not created automatically. On your machine:

1. `gh auth login` (once)
2. From this directory:  
   `gh repo create RootRecord/Doc-Repo --public --source . --remote origin --push`  
   If the organization or name differs, swap `RootRecord/Doc-Repo` for your target (for example `YOUR_USER/Doc-Repo`).

If the empty repo already exists on GitHub:  
`git remote add origin https://github.com/RootRecord/Doc-Repo.git`  
`git push -u origin main`
