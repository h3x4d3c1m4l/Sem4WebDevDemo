# Demo frontend

This is a demo frontend for [my workshop](https://h3x4d3c1m4l.github.io/cicd-with-github-workshop-slides/). Is has been created with the following command (ran from the `Frontend` folder):

```bash
npx create-react-router@latest .
```

Additionally, SSR (Server Side Rendering) has been disabled (in [react-router.config.ts](./react-router.config.ts)) to ensure this frontend runs as a classic SPA (Single Page Application) which can be deployed to an Azure Static Web App.

## Running locally

```bash
npm i # Only needed once
npm run start
```

## Deploying to the cloud

This repository contains a [GitHub Actions workflow](../.github/workflows/deploy-to-azure.yml) to demonstrate how this frontend can be deployed automatially to Azure.

Don't forget to add the `AZURE_DEPLOYMENT_TOKEN` secret to your GitHub repository.
