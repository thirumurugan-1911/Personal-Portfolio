# 🌐 Thirumurugan B — Personal Portfolio Website

A fully accessible, SEO-optimized single-page personal portfolio website built with **HTML5**, **CSS3**, and **vanilla JavaScript**.

---

## 📸 Preview

> A clean, responsive portfolio showcasing skills, projects, and a contact form — fully keyboard-navigable and Lighthouse-ready.

---

## ✨ Features

- **Semantic HTML5** — Proper use of `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>` tags
- **Accessibility (WCAG 2.1)** — ARIA labels, roles, skip links, focus management, and visible focus rings
- **SEO Optimized** — Meta tags, Open Graph, Twitter Cards, and canonical URL included
- **Responsive Design** — Works on all screen sizes (mobile, tablet, desktop)
- **Contact Form** — Client-side validated form with accessible error messages
- **Keyboard Navigation** — Full Tab-key support with `aria-current` page indicators
- **Reduced Motion Support** — Respects `prefers-reduced-motion` user preference
- **Zero Dependencies** — Pure HTML/CSS/JS, no frameworks or libraries required

---

## 🗂️ Project Structure

```
portfolio/
│
├── portfolio_fixed.html    # Main portfolio file (single self-contained file)
└── README.md               # Project documentation
```

---

## 🏗️ HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
  <head>           <!-- SEO meta, OG tags, Twitter Cards, canonical -->
  <body>
    <a class="skip-link">Skip to main content</a>

    <header role="banner">
      <nav role="navigation" aria-label="Main navigation">
        <ul>
          <li><a aria-current="page">Home</a></li>
          ...
        </ul>
      </nav>
    </header>

    <main id="main-content">
      <section aria-labelledby="...">
        <h1>Thirumurugan B</h1>
        <article role="listitem"> ... </article>
      </section>

      <section id="contact">
        <form aria-label="Contact form" novalidate>
          <input aria-required="true" aria-describedby="name-error">
          <span class="error-msg" role="alert">...</span>
        </form>
      </section>
    </main>

    <footer role="contentinfo">
      <nav aria-label="Footer navigation"> ... </nav>
    </footer>
  </body>
</html>
```

---

## 🚀 Getting Started

### Option 1 — Open Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/portfolio.git
   ```
2. Open `portfolio_fixed.html` in any modern browser — no server required.

### Option 2 — Deploy with GitHub Pages

1. Go to your repository **Settings → Pages**
2. Set the source branch to `main` and folder to `/ (root)`
3. Your portfolio will be live at:
   ```
   https://your-username.github.io/portfolio/
   ```

---

## 🧪 Testing & Validation

| Test | Tool |
|------|------|
| Accessibility | Chrome DevTools → Lighthouse |
| HTML Validation | [W3C Validator](https://validator.w3.org/) |
| WCAG Compliance | [WAVE Accessibility Tool](https://wave.webaim.org/) |
| Keyboard Nav | Press `Tab` key through the page |
| Responsive | Chrome DevTools → Toggle Device Toolbar |

---

## 🐛 Bugs Fixed

| Bug | Cause | Fix |
|-----|-------|-----|
| Unclosed `<head>` tag | Regex counted "header" text as `<head>` tags | Rebuilt with proper tag matching |
| Broken apostrophe in content | Used `\'` escape in raw string | Replaced with plain text |
| Unclosed `<style>` tag | CSS property names like `font-style` triggered false match | Proper regex for actual `<style>` tags |
| Imbalanced quotes | Mixed `'` and `"` in inline styles | Standardized all quotes |

---

## 🌍 Browser Support

| Browser | Supported |
|---------|-----------|
| Chrome | ✅ |
| Firefox | ✅ |
| Safari | ✅ |
| Edge | ✅ |
| Opera | ✅ |

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Thirumurugan B**

- 📧 Contact via the form on the portfolio page
- 🔗 GitHub: (https://github.com/thirumurugan-1911)
- 💼 LinkedIn: ((https://www.linkedin.com/in/thirumurugan-b-302800380))

---

> Built with ❤️ using pure HTML, CSS, and JavaScript — no frameworks, no bloat.
