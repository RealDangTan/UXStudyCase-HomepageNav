# GitHub Pages Deployment Guide

This guide explains how to complete the GitHub Pages deployment for this repository.

## Steps to Enable GitHub Pages

### 1. Repository Settings
1. Go to your repository on GitHub: `https://github.com/RealDangTan/UXStudyCase-HomepageNav`
2. Click on **Settings** tab
3. Scroll down to **Pages** section in the left sidebar

### 2. Configure Pages Source
1. Under **Source**, select **GitHub Actions**
2. The workflow in `.github/workflows/pages.yml` will handle the deployment

### 3. Enable Workflow Permissions
1. Go to **Settings** → **Actions** → **General**
2. Under **Workflow permissions**, select **Read and write permissions**
3. Check **Allow GitHub Actions to create and approve pull requests**
4. Click **Save**

### 4. Trigger Deployment
The deployment will automatically trigger when:
- Changes are pushed to the main branch
- Or you can manually trigger it from the **Actions** tab

### 5. Access Your Site
Once deployed, your site will be available at:
**https://realdangtan.github.io/UXStudyCase-HomepageNav/**

## Manual Deployment (Alternative)

If you prefer manual deployment without GitHub Actions:

1. Go to **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose **main** branch and **/ (root)** folder
4. Click **Save**

The site will be deployed directly from the main branch.

## Troubleshooting

### Common Issues:
1. **404 Error**: Check that `index.html` is in the root directory
2. **Workflow Fails**: Verify workflow permissions are enabled
3. **Site Not Updating**: Clear browser cache or wait for CDN update

### Verifying Deployment:
1. Check the **Actions** tab for workflow status
2. Look for green checkmarks indicating successful deployment
3. Visit the live URL to test functionality

## Custom Domain (Optional)

To use a custom domain:
1. Add a `CNAME` file to the repository root with your domain
2. Configure DNS settings with your domain provider
3. Update the custom domain in Pages settings

---

Your UX Study Case homepage is now ready for the world to see! 🚀