# CVPR 2026 Workshop - Med-Reasoner

Website for the CVPR 2026 Workshop on Medical Reasoning with Vision Language Foundation Models (Med-Reasoner).

## Deploying to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **+** icon in the top right and select **New repository**
3. Name your repository (e.g., `med-reasoner-cvpr2026` or `cvpr2026` for a cleaner URL)
4. Make it **Public** (required for free GitHub Pages)
5. **Don't** initialize with README (we already have files)
6. Click **Create repository**

### Step 2: Push Your Website Files

Open a terminal in this folder and run:

```bash
git init
git add .
git commit -m "Initial commit: Med-Reasoner CVPR 2026 workshop website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repository name.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (gear icon)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click **Save**

### Step 4: Access Your Website

After a few minutes, your website will be available at:
- `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

## Customizing the Website

### Adding Speaker/Organizer Photos

1. Add photos to `assets/img/speakers/` or `assets/img/organisers/`
2. Update the `<img src="...">` tags in `index.html` with the correct filenames
3. Recommended photo size: 200x200 pixels, square aspect ratio

### Updating Content

- **Home page**: Edit `index.html`
- **Call for Papers**: Edit `call_for_paper.html`
- **Styling**: Edit `assets/css/style.css`

### Adding Speaker Links

To make speaker cards clickable, wrap them in anchor tags:

```html
<a href="https://scholar.google.com/..." class="col-lg-3 col-md-4 col-sm-6 mb-4">
    <div class="card person-card h-100">
        ...
    </div>
</a>
```

## File Structure

```
med-reasoner-cvpr2026/
├── index.html              # Main homepage
├── call_for_paper.html     # Call for papers page
├── README.md               # This file
└── assets/
    ├── css/
    │   └── style.css       # Custom styles
    └── img/
        ├── speakers/       # Speaker photos
        └── organisers/     # Organizer photos
```

## Updating Important Dates

Edit the dates table in `call_for_paper.html`:

```html
<tr>
    <td class="date-label"><strong>Submission deadline</strong></td>
    <td class="date-value">March 24, 2026 (23:59 AoE)</td>
</tr>
```

## Adding the OpenReview Link

Once you have your OpenReview portal URL, update the link in `call_for_paper.html`:

```html
<a href="https://openreview.net/group?id=YOUR_WORKSHOP_ID" class="btn btn-primary btn-lg">
    Submit on OpenReview
</a>
```

## Need Help?

For any questions about the workshop website, contact: [your-email@example.com]
