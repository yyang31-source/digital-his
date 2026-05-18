# Website Folder

This folder contains files for your GitHub Pages website.

## Basic Structure

```
website/
├── index.html         Main page
├── about.html         About/methodology page
├── css/
│   └── style.css      Styles
├── js/
│   └── main.js        JavaScript (if needed)
├── images/            Images and visualizations
└── data/              Data files for interactive elements
```

## GitHub Pages Setup

1. **Enable GitHub Pages** in repository settings:
   - Settings → Pages → Source: main branch, /website folder
   - Or use root folder if you prefer

2. **Your site will be available at**:
   - `https://username.github.io/project-name/`

## Minimal Template

See `index.html` for a starter template.

### index.html (Basic Structure)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Project Title</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <header>
        <h1>Your Project Title</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="about.html">About</a>
        </nav>
    </header>
    
    <main>
        <section>
            <h2>Introduction</h2>
            <p>Your project description...</p>
        </section>
        
        <section>
            <h2>Findings</h2>
            <!-- Your visualizations, maps, or analysis -->
        </section>
    </main>
    
    <footer>
        <p>&copy; 2026 Your Name | Hist 501D</p>
    </footer>
</body>
</html>
```

## Embedding Content

### Images/Visualizations

```html
<img src="images/visualization.png" alt="Description of image">
```

### Interactive Maps

If using Leaflet/Folium:
```html
<div id="map" style="height: 500px;"></div>
<script src="map.js"></script>
```

### Jupyter Notebook Exports

Convert notebooks to HTML:
```bash
jupyter nbconvert --to html notebook.ipynb
```

Then link to them or embed sections.

## Accessibility

Remember to:
- Add `alt` text to all images
- Use semantic HTML tags (`<header>`, `<nav>`, `<main>`, `<footer>`)
- Ensure good color contrast
- Test on mobile devices

## Testing Locally

Open `index.html` in your browser to test before pushing to GitHub.

Or use Python's built-in server:
```bash
cd website
python -m http.server 8000
```

Then visit `http://localhost:8000`

## Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [HTML/CSS Tutorials](https://www.w3schools.com/)
- [Web Accessibility Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
