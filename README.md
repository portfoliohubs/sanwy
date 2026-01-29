# Hugo Static Website

This is a static website built with Hugo for GitHub Pages deployment.

## Files Structure

- `index.html` - Main HTML file with all content, CSS, and JavaScript
- `config.toml` - Hugo configuration
- `.github/workflows/deploy.yml` - GitHub Actions workflow for deployment

## Setup Instructions

1. Update `config.toml` with your GitHub username and repository name:
   ```toml
   baseURL = 'https://yourusername.github.io/your-repo-name'
   ```

2. Push to GitHub repository

3. Enable GitHub Pages in repository settings

4. The workflow will automatically build and deploy your site

## Local Development

To test locally, install Hugo first:
```bash
# Windows (using Chocolatey)
choco install hugo

# Or download from https://github.com/gohugoio/hugo/releases
```

Then run:
```bash
hugo server
```

## Deployment

The GitHub Actions workflow will automatically:
- Build the site with `hugo --minify`
- Deploy to GitHub Pages when pushing to main branch

No theme is used - the site uses a single HTML file with embedded CSS and JavaScript.
