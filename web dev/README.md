# Food Website Frontend

A responsive multi-page restaurant/food website built with plain HTML, CSS, and JavaScript. The project is ready to run locally and deploy as a static frontend to platforms such as Vercel, Netlify, Render Static Sites, or GitHub Pages.

## Pages

- `index.html` - Home page
- `about.html` - About page
- `menu.html` - Menu page
- `products.html` - Products page
- `review.html` - Customer reviews page
- `contact.html` - Contact page
- `blog.html` - Blog page

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Font Awesome CDN
- Google Fonts CDN

## Project Structure

```text
.
├── image/              # Local image assets
├── about.html
├── blog.html
├── contact.html
├── index.html
├── menu.html
├── products.html
├── review.html
├── script.js           # Header interactions
├── server.js           # Local static server
├── style.css           # Global styles
├── package.json
├── netlify.toml
├── vercel.json
└── README.md
```

## Run Locally

Make sure Node.js is installed, then run:

```bash
npm start
```

Open:

```text
http://127.0.0.1:5500
```

You can choose a different port:

```bash
npm start -- --port 3000
```

## Deployment

This is a static frontend. No build step is required.

### Vercel

1. Import the repository in Vercel.
2. Keep the framework preset as `Other`.
3. Leave the build command empty or use `npm run build`.
4. Set the output directory to `.`.

The included `vercel.json` enables clean URLs and asset caching.

### Netlify

1. Import the repository in Netlify.
2. Leave the build command empty or use `npm run build`.
3. Set the publish directory to `.`.

The included `netlify.toml` already defines the publish directory and cache headers.

### GitHub Pages

1. Push the project to a GitHub repository.
2. Go to repository Settings -> Pages.
3. Select the branch and root folder.
4. Save and wait for GitHub Pages to publish the site.

The included `.nojekyll` file helps GitHub Pages serve static assets as-is.

## Notes

- The site uses CDN resources for fonts and icons, so internet access is required for those assets to load.
- Images are stored in the `image/` folder and referenced directly from the HTML/CSS files.
- The project has no production dependencies.
