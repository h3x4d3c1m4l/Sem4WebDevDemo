# Demo backend

This is a demo backend for [my workshop](https://h3x4d3c1m4l.github.io/cicd-with-github-workshop-slides/). Is has been created with the following command (ran from the `Backend` folder):

```bash
npx express-generator . --no-view
```

## Running locally

```bash
npm i # Only needed once
npm run start
```

## Deploying to the cloud

This repository contains a [GitHub Actions workflow](../.github/workflows/deploy-to-azure.yml) to demonstrate how this backend can be deployed automatially to Azure.

Don't forget to add the `AZURE_PUBLISH_PROFILE` secret to your GitHub repository.
