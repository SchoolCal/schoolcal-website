This is the SchoolCal marketing website built with [Next.js](https://nextjs.org).

## Getting Started

### Prerequisites

- Node.js (see `.nvmrc` for version)
- Sanity CMS credentials

### Environment Setup

Copy the example environment file and fill in your credentials:

```bash
cp .env.local.example .env.local
```

Required environment variables:
- `NEXT_PUBLIC_SANITY_PROJECT_ID` - Sanity project ID
- `NEXT_PUBLIC_SANITY_DATASET` - Sanity dataset (e.g., `production`)
- `SANITY_API_READ_TOKEN` - Sanity API read token

### Development

```bash
nvm use
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser.

## Deployment

The site is automatically deployed to Azure Static Website hosting on push to `main` branch via GitHub Actions. See `.github/workflows/deploy.yml` for details.
