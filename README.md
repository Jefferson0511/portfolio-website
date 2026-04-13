# Jefferson Kingston — Visual Portfolio

A minimal photography and design portfolio, built for GitHub Pages.

## Quick Setup (5 minutes)

### 1. Create the GitHub repo
- Go to [github.com/new](https://github.com/new)
- Name it: `portfolio` (or `jeffersonkingston.github.io` for a custom domain)
- Set it to **Public**
- Click **Create repository**

### 2. Upload your files
- Upload `index.html` to the root of the repo
- Create a folder called `photos/` and upload your images there

### 3. Enable GitHub Pages
- Go to **Settings** → **Pages**
- Under "Source", select **Deploy from a branch**
- Select the **main** branch, root `/`
- Click **Save**
- Your site will be live at: `https://YOUR-USERNAME.github.io/portfolio/`

### 4. Add your photos

Open `index.html` and replace the placeholder cards with real ones. Each photo card follows this format:

```html
<div class="photo-card"
     data-title="Keynote Speaker"
     data-category="Youth Conference 2024"
     onclick="openLightbox(this)">
    <img src="photos/keynote-speaker.jpg"
         alt="Speaker at Youth Conference 2024" loading="lazy">
    <div class="overlay">
        <span>Youth Conference 2024</span>
        <h3>Keynote Speaker</h3>
    </div>
</div>
```

**Just change:**
- `src="photos/your-filename.jpg"` → your actual image path
- `data-title` → what the photo shows
- `data-category` → the event name
- `alt` → description for accessibility

Delete any leftover `placeholder` cards when you're done.

## Photo Tips for Best Results

- **File size**: Keep images under 1.5MB each (compress at [tinypng.com](https://tinypng.com))
- **Naming**: Use lowercase, dashes instead of spaces (`youth-conf-keynote.jpg`)
- **Aspect ratio**: 4:3 works best with the grid, but any ratio will work
- **Count**: 8–12 photos is the sweet spot. Quality over quantity.

## Adding Canva Designs Later

The "Graphic Design" section is already built into the page. When ready, just add cards to the `designGrid` section using the same format — export your Canva designs as PNG/JPG and drop them in a `designs/` folder.

## Customization

The site uses CSS variables at the top of the `<style>` block. You can tweak:
- `--bg` → background color
- `--text` → main text color
- `--text-muted` → subtitle color

The About section text can be edited directly in the HTML.