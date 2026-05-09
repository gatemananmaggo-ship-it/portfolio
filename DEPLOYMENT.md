# Deployment Guide (Static Site)

This guide explains how to deploy your portfolio website to the internet for free using **GitHub Pages** or **Vercel**. Since this is now a static site (HTML/CSS/JS only), deployment is extremely simple.

## Prerequisites
1.  **GitHub Account**: You need a GitHub account to host your code.
2.  **Git Installed**: You already have this.

## Step 1: Push to GitHub
1.  Initialize a git repository (if you haven't already):
    ```bash
    git init
    git add .
    git commit -m "Convert to static site"
    ```
2.  Create a new repository on [GitHub](https://github.com/new).
3.  Push your code:
    ```bash
    git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
    git branch -M main
    git push -u origin main
    ```

## Step 2: Choose Your Hosting

### Option A: GitHub Pages (Easiest)
1.  Go to your repository on GitHub.
2.  Click **Settings** -> **Pages**.
3.  Under **Build and deployment**, set **Source** to "Deploy from a branch".
4.  Select `main` branch and `/root` folder, then click **Save**.
5.  Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/` in a few minutes.

### Option B: Vercel (Fastest & Best Features)
1.  Go to [Vercel](https://vercel.com/) and sign up with GitHub.
2.  Click **"Add New..."** -> **"Project"**.
3.  Import your repository.
4.  Vercel will automatically detect it as a static project.
5.  Click **Deploy**.

## Local Development
Since there is no longer a `server.js`, you can view your site locally by:
-   **Opening the file**: Just double-click `index.html` in your file explorer.
-   **Live Server (VS Code)**: Install the "Live Server" extension and click "Go Live" at the bottom right.
