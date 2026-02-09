# KEC × GUVI DevOps Partnership Page

> An attractive, modern website showcasing the partnership between Kongu Engineering College and GUVI for DevOps training.

## Features

✨ **Modern Design**
- Responsive dark theme with gradient backgrounds
- Glass-morphism effects with animations
- Interactive countdown timer with seconds
- Smooth scroll animations

📚 **Content**
- Partnership details with highlights
- Dual learning methodology (Theory + Practical)
- Course modules and features
- Student benefits and testimonials
- FAQ section with accordions
- Success stories and statistics
- Industry partners showcase

## Local Development

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Git (for version control)
- Text editor or IDE (VS Code recommended)

### Running Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/kec-guvi-partnership.git
   cd kec-guvi-partnership
   ```

2. Open the HTML file in your browser:
   - Double-click `home.html` OR
   - Use `python -m http.server 8000` (Python 3) and visit `http://localhost:8000`

## 🚀 Deployment Guide

### Step 1: Push to GitHub

1. **Initialize Git (if not already done)**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: KEC-GUVI partnership website"
   ```

2. **Create a GitHub Repository**:
   - Go to [github.com](https://github.com) and log in
   - Click "+" → "New repository"
   - Name: `kec-guvi-partnership`
   - Description: "DevOps partnership website between KEC and GUVI"
   - Choose Public (for Netlify to access)
   - Click "Create repository"

3. **Connect and Push**:
   ```bash
   git remote add origin https://github.com/your-username/kec-guvi-partnership.git
   git branch -M main
   git push -u origin main
   ```

### Step 2: Deploy on Netlify

#### Option A: Netlify UI (Recommended for Beginners)

1. **Sign Up / Log In**:
   - Visit [netlify.com](https://netlify.com)
   - Click "Sign up" → Choose "GitHub"
   - Authorize Netlify to access GitHub

2. **Connect Repository**:
   - Click "Add new site" → "Import an existing project"
   - Select GitHub
   - Find and select `kec-guvi-partnership` repository

3. **Configure Build Settings**:
   - Build command: Leave empty (it's a static site)
   - Publish directory: `.` (root folder)
   - Click "Deploy site"

4. **Wait for Deployment**:
   - Netlify will automatically deploy
   - You'll get a site URL like: `https://your-site-name.netlify.app`

#### Option B: Using GitHub Actions Workflow

The workflow file (`.github/workflows/deploy.yml`) is already configured!

1. **Add Netlify Secrets to GitHub**:
   - Go to your GitHub repository
   - Settings → Secrets and variables → Actions
   - Click "New repository secret"

2. **Add NETLIFY_AUTH_TOKEN**:
   - Visit [netlify.com/user/applications](https://app.netlify.com/user/applications)
   - Click "New access token"
   - Copy the token
   - Go back to GitHub Secrets and add it as `NETLIFY_AUTH_TOKEN`

3. **Add NETLIFY_SITE_ID**:
   - Create a site on Netlify first
   - Go to Site settings → General
   - Copy "Site ID"
   - Add it to GitHub Secrets as `NETLIFY_SITE_ID`

4. **Trigger Deployment**:
   ```bash
   git push
   ```
   - GitHub Actions will automatically run and deploy to Netlify!

### Step 3: Custom Domain (Optional)

1. **In Netlify Dashboard**:
   - Click on your site
   - Go to "Domain settings"
   - Click "Add custom domain"
   - Enter your domain (e.g., `kec-guvi.com`)

2. **Update DNS** (with your domain provider):
   - Follow Netlify's DNS instructions
   - Point your domain to Netlify

## File Structure

```
kec-guvi-partnership/
├── home.html                    # Main website file
├── handshake.png               # Partnership logo icon
├── README.md                    # This file
└── .github/
    └── workflows/
        └── deploy.yml          # GitHub Actions workflow
```

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with gradients and animations
- **JavaScript** - Interactivity and countdown timer
- **Font Awesome** - Icon library
- **Git** - Version control
- **GitHub Actions** - CI/CD automation
- **Netlify** - Hosting platform

## Environment Variables

No environment variables needed for this static site!

## Troubleshooting

### Deployment Failed?
- Check GitHub Actions logs: Repository → Actions tab
- Verify Netlify secrets are correctly set
- Ensure `home.html` is in the root directory

### Website Not Showing Images?
- Check relative paths for images
- Ensure `handshake.png` is in the same directory as `home.html`

### Domain Not Working?
- DNS changes take 24-48 hours to propagate
- Verify DNS records in Netlify and your domain provider

## Support

For issues or questions:
- Check Netlify documentation: [docs.netlify.com](https://docs.netlify.com)
- GitHub Actions help: [github.com/actions](https://github.com/actions)
- Contact support through respective platforms

## License

This project is licensed under the MIT License - feel free to use it for educational purposes.

---

**🎉 Happy Deploying!**

