# GitHub Pages Deployment Instructions

This package contains a static website build optimized for GitHub Pages deployment. Follow these instructions to deploy the site to your GitHub repository.

## Prerequisites

- A GitHub account
- Git installed on your local machine

## Deployment Steps

1. **Create a new repository on GitHub**
   - Go to [GitHub](https://github.com) and sign in
   - Click the "+" icon in the top right corner and select "New repository"
   - Name your repository `ai-agent-alternatives` (important: this name must match the base path in the build)
   - Make the repository public
   - Do not initialize it with a README, .gitignore, or license

2. **Initialize a local Git repository and push the build**
   - Extract this zip file to a local directory
   - Open a terminal/command prompt and navigate to the extracted directory
   - Run the following commands:

   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/ai-agent-alternatives.git
   git push -u origin main
   ```

   (Replace `YOUR_USERNAME` with your actual GitHub username)

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click on "Settings"
   - Scroll down to the "GitHub Pages" section
   - Under "Source", select "main" branch and "/" (root) folder
   - Click "Save"

4. **Access your website**
   - After a few minutes, your site will be available at:
   - `https://YOUR_USERNAME.github.io/ai-agent-alternatives/`

## Troubleshooting

- If assets aren't loading correctly, ensure the repository name exactly matches `ai-agent-alternatives`
- If you prefer a different repository name, you'll need to update the `base` path in `vite.config.ts` and rebuild

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Vite Deployment Guide](https://vitejs.dev/guide/static-deploy.html#github-pages)
