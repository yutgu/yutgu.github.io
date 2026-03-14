# Yuting Gu — Academic Website

Personal academic website hosted on GitHub Pages.

## Setup Instructions

### 1. Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name the repository `yutgu.github.io` (must match your GitHub username)
3. Set it to **Public**
4. Click **Create repository**

### 2. Upload Files

Upload all files from this folder to the repository:

```
index.html
research.html
cv.html
teaching.html
about.html
resources.html
style.css
photo.jpg          ← Add your headshot photo here
cv.pdf             ← Add your CV PDF here
```

You can do this via the GitHub web interface (drag and drop) or via command line:

```bash
cd /path/to/this/folder
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/yutgu/yutgu.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Branch: `main`, folder: `/ (root)`
4. Click **Save**

Your site will be live at: **https://yutgu.github.io**

It may take 1–2 minutes for the first deployment.

### 4. Add Your Photo and CV

Replace the placeholder references:
- `photo.jpg` — your headshot (the one from your Google Sites)
- `cv.pdf` — your current CV

### 5. Custom Domain (Optional)

If you want a custom domain like `yutinggu.com`:

1. Buy a domain from a registrar (Namecheap, Google Domains, etc.)
2. In the repo, create a file called `CNAME` containing just your domain:
   ```
   yutinggu.com
   ```
3. In your domain registrar's DNS settings, add:
   - A record: `185.199.108.153`
   - A record: `185.199.109.153`
   - A record: `185.199.110.153`
   - A record: `185.199.111.153`
   - CNAME record: `www` → `yutgu.github.io`

## Updating Content

Edit any `.html` file directly on GitHub (click the file → pencil icon → commit). Changes go live within a minute.

## File Structure

```
├── index.html        Home page
├── research.html     Research projects, publications, presentations
├── cv.html           Embedded CV PDF
├── teaching.html     Teaching history
├── about.html        Personal bio
├── resources.html    Useful links
├── style.css         Shared stylesheet
├── photo.jpg         Your headshot
├── cv.pdf            Your CV
└── README.md         This file
```
