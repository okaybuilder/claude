# Israel Art Shop - Presentation

A beautiful HTML/CSS presentation built with Reveal.js for Israel Art Shop.

## 🚀 Quick Start

1. **Open the presentation:**
   - Simply open `index.html` in your web browser
   - Or use a local server for best results:
     ```bash
     # Python 3
     python -m http.server 8000

     # Python 2
     python -m SimpleHTTPServer 8000

     # Node.js (if you have http-server installed)
     npx http-server
     ```
   - Then visit: `http://localhost:8000`

2. **Navigate the slides:**
   - **Next/Previous:** Arrow keys, Space, or on-screen controls
   - **Overview mode:** Press ESC
   - **Fullscreen:** Press F
   - **Presenter notes:** Press S (opens separate window)
   - **Zoom:** Alt+Click (Windows/Linux) or Ctrl+Click (Mac)

## 📁 File Structure

```
presentation/
├── index.html          # Main presentation file
├── style.css           # Custom styling
└── README.md          # This file
```

## 🎨 Customization Guide

### Changing Content

Edit `index.html` and modify the content inside `<section>` tags:

```html
<section>
    <h2>Your Title</h2>
    <p>Your content here</p>
</section>
```

### Adding Images

```html
<section>
    <h2>Gallery</h2>
    <img src="path/to/image.jpg" alt="Description" style="max-width: 80%;">
</section>
```

### Creating Vertical Slides (Nested)

```html
<section>
    <section>
        <h2>Main Topic</h2>
    </section>
    <section>
        <h2>Subtopic 1</h2>
    </section>
    <section>
        <h2>Subtopic 2</h2>
    </section>
</section>
```

### Adding Fragments (Step-by-step reveals)

```html
<ul>
    <li class="fragment">Appears first</li>
    <li class="fragment">Appears second</li>
    <li class="fragment">Appears third</li>
</ul>
```

### Customizing Colors

Edit the CSS variables in `style.css`:

```css
:root {
    --primary-color: #0078d4;      /* Main blue */
    --accent-color: #f4a261;       /* Orange accent */
    --text-color: #ffffff;         /* White text */
    --background-dark: #1a1a2e;    /* Dark background */
    --background-light: #16213e;   /* Lighter background */
}
```

### Changing Transition Effects

In `index.html`, modify the Reveal.initialize settings:

```javascript
Reveal.initialize({
    transition: 'slide',  // Options: none/fade/slide/convex/concave/zoom
    // ... other settings
});
```

## ✨ Features Included

- ✅ Responsive design (mobile-friendly)
- ✅ Smooth transitions and animations
- ✅ Custom color scheme
- ✅ Fragment animations
- ✅ Keyboard navigation
- ✅ Touch support for mobile
- ✅ Overview mode (ESC)
- ✅ Progress bar
- ✅ Slide numbers
- ✅ Zoom functionality

## 🎯 Slide Sections

1. **Title Slide** - Introduction
2. **About Us** - Company information
3. **Our Products** - Product showcase with grid layout
4. **Featured Artists** - Artist profiles
5. **Why Choose Us** - Key benefits
6. **Gallery Showcase** - Vertical slides for collections
7. **Customer Testimonials** - Social proof
8. **Contact** - Contact information
9. **Thank You** - Closing slide

## 🔧 Advanced Features

### Adding Backgrounds

```html
<section data-background-color="#ff0000">
    <h2>Slide with red background</h2>
</section>

<section data-background-image="image.jpg">
    <h2>Slide with image background</h2>
</section>

<section data-background-video="video.mp4">
    <h2>Slide with video background</h2>
</section>
```

### Speaker Notes

```html
<section>
    <h2>Slide Title</h2>
    <aside class="notes">
        These notes are only visible in presenter mode (press S)
    </aside>
</section>
```

### Auto-Animate

```html
<section data-auto-animate>
    <h2>Slide 1</h2>
</section>
<section data-auto-animate>
    <h2>Slide 2</h2>
</section>
```

## 📱 Export to PDF

1. Open the presentation in Chrome/Chromium
2. Add `?print-pdf` to the URL (e.g., `http://localhost:8000?print-pdf`)
3. Print to PDF using browser's print function

## 🌐 Hosting Online

You can host this presentation on:
- **GitHub Pages:** Push to a repo and enable Pages
- **Netlify:** Drag and drop the folder
- **Vercel:** Deploy with one click
- **Any web server:** Upload the files

## 📚 Resources

- [Reveal.js Documentation](https://revealjs.com/)
- [Reveal.js GitHub](https://github.com/hakimel/reveal.js)
- [More Themes](https://revealjs.com/themes/)

## 💡 Tips

- Keep text minimal on each slide
- Use high-quality images
- Test on different screen sizes
- Practice presenter mode (press S)
- Use fragments to control information flow
- Don't overuse animations

## 🛠️ Troubleshooting

**Presentation not loading?**
- Check browser console for errors
- Make sure you're using a modern browser
- Try using a local server instead of opening file directly

**Fonts look different?**
- Check your internet connection (fonts load from CDN)
- Or download fonts locally and update CSS

**Images not showing?**
- Check file paths are correct
- Use relative paths (e.g., `images/photo.jpg`)

---

*Created for Israel Art Shop*
*Powered by Reveal.js*
