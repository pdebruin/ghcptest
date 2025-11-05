# Azure Static Web Apps Deployment

This document describes how to deploy the MARP presentation to Azure Static Web Apps.

## Overview

The MARP presentation can be automatically deployed to Azure Static Web Apps using the GitHub Actions workflow defined in `.github/workflows/deploy-marp-azure-static-web-apps.yml`.

## Prerequisites

Before you can deploy to Azure Static Web Apps, you need to:

1. **Create an Azure Static Web Apps resource**:
   - Sign in to the [Azure Portal](https://portal.azure.com)
   - Create a new Static Web App resource
   - Choose "GitHub" as the deployment source
   - Authorize Azure to access your GitHub account
   - Select this repository and the `main` branch

2. **Configure the deployment token**:
   - After creating the Static Web App, navigate to your resource in the Azure Portal
   - Go to **Settings** > **Configuration** > **Deployment tokens**
   - Copy the deployment token
   - In this GitHub repository, go to **Settings** > **Secrets and variables** > **Actions**
   - Create a new repository secret named `AZURE_STATIC_WEB_APPS_API_TOKEN`
   - Paste the deployment token as the value

## Workflow Configuration

The workflow is configured with the following settings:

- **Trigger**: Runs on push to `main` branch when files in `marp/` directory change
- **Build**: Compiles `slides.md` with the custom theme to an HTML file
- **Deploy**: Uploads the built presentation to Azure Static Web Apps

### Workflow Parameters

- `app_location`: `dist` - The folder containing the built HTML presentation
- `skip_app_build`: `true` - We handle the build ourselves using MARP CLI
- `output_location`: `""` - Empty because we already have the final build output

## Manual Deployment

You can manually trigger a deployment using the GitHub Actions UI:

1. Go to the **Actions** tab in this repository
2. Select the "Deploy MARP Presentation to Azure Static Web Apps" workflow
3. Click "Run workflow"
4. Select the branch and click "Run workflow"

## Viewing the Deployed Site

After a successful deployment:

1. Navigate to your Static Web App in the Azure Portal
2. Click on the **URL** link in the Overview section to view your deployed presentation

The URL will be in the format: `https://<your-app-name>.azurestaticapps.net`

## Pull Request Previews

When you open a pull request that modifies files in the `marp/` directory:

- A preview deployment is automatically created
- The preview URL is posted as a comment on the pull request
- When the pull request is closed, the preview deployment is removed

## Troubleshooting

### Deployment Token Issues

If the deployment fails with authentication errors:
- Verify that the `AZURE_STATIC_WEB_APPS_API_TOKEN` secret is correctly set
- Ensure the token hasn't expired or been regenerated in Azure
- Check that the secret name matches exactly (case-sensitive)

### Build Failures

If the MARP compilation fails:
- Check that the `slides.md` and `theme.css` files are valid
- Review the GitHub Actions logs for specific error messages
- Ensure Node.js 20 is compatible with the version of MARP CLI being used

## Resources

- [Azure Static Web Apps Documentation](https://learn.microsoft.com/en-us/azure/static-web-apps/)
- [MARP Documentation](https://marp.app/)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
