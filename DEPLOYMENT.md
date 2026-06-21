# Deploying Jasmeh Robotics Portfolio

This folder is the deployment-ready version of the website.

## Local preview

From this folder:

```bash
python3 -m http.server 4180
```

Open:

```txt
http://localhost:4180/
```

## First GitHub push

Sign in to GitHub:

```bash
gh auth login
```

If Git does not know your name/email yet:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Commit the site:

```bash
git commit -m "Initial robotics portfolio site"
```

Create the GitHub repository and push:

```bash
gh repo create jasmehrobotics --public --source=. --remote=origin --push
```

## Vercel deployment

1. Go to https://vercel.com/new
2. Import the `jasmehrobotics` GitHub repository.
3. Use these settings:
   - Framework Preset: Other
   - Build Command: leave blank
   - Output Directory: leave blank or `.`
4. Deploy.

The site should be available at:

```txt
https://jasmehrobotics.vercel.app
```

