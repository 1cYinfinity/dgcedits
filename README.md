# DGC Edits — Official Website

> Professional Video Editing & Post-Production Services  
> Mumbai, India · Est. 2017 · [dgcedits.com](https://dgcedits.com)

---

## Overview

This is the official website for **DGC Edits**, a full-service post-production company powered by DGC Film Works. The site is built as a single-page HTML application — no frameworks, no build tools, no dependencies.

---

## Pages

| Page | Description |
|------|-------------|
| **Home** | Hero section, services, process steps, pricing plans, testimonials |
| **Portfolio** | Filterable work showcase (Commercial, Reels, Motion, Vlogs, Corporate) |
| **About** | Company story, vision/mission, team members, values |
| **Contact** | Contact form, office info, social links |

---

## Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, Grid, Flexbox, animations
- **Vanilla JavaScript** — Page routing, portfolio filtering, form handling
- **Google Fonts** — Syne (headings) + DM Sans (body)

> No frameworks. No npm. No build step. Just one `.html` file.

---

## File Structure

```
dgcedits/
├── dgcedits.html      # Entire website (HTML + CSS + JS)
└── README.md          # This file
```

---

## Responsive Breakpoints

| Breakpoint | Layout |
|------------|--------|
| `1024px+`  | Full desktop — 3-column grids, side-by-side layouts |
| `≤ 1024px` | Tablet — 2-column grids, adjusted spacing |
| `≤ 768px`  | Mobile — hamburger menu, stacked layouts |
| `≤ 480px`  | Small mobile — single column, compact spacing |

---

## Deployment

### Netlify (Recommended)
1. Go to [netlify.com](https://netlify.com) and create a free account
2. Drag & drop `dgcedits.html` onto the dashboard
3. Connect your custom domain `dgcedits.com` in Domain Settings
4. Update nameservers at your domain registrar

### GitHub Pages
1. Go to repo **Settings → Pages**
2. Set source branch to `main`, folder to `/ (root)`
3. Rename `dgcedits.html` to `index.html`
4. Site will be live at `https://yourusername.github.io/repo-name`

### Any Static Host
Upload `dgcedits.html` (rename to `index.html`) to any static hosting provider — Vercel, Cloudflare Pages, cPanel file manager, etc.

> ⚠️ Always use **HTTPS**. Netlify and Vercel provide free SSL automatically.

---

## Customization

### Update Contact Info
Search for the following in `dgcedits.html` and replace with your details:

```
connect@dgcedits.com        → your email
+91 79052 79486             → your phone
Link Road, Andheri West     → your address
```

### Add Real Portfolio Videos
Find `portfolioItems` array in the `<script>` section and add your video URLs and thumbnail images.

### Enable Real Contact Form Emails
The contact form currently shows an alert. To receive actual emails, integrate [Formspree](https://formspree.io) (free):

1. Create a free account at formspree.io
2. Get your form endpoint URL
3. Replace the `handleSubmit()` function in the script section:

```js
async function handleSubmit() {
  const data = {
    name:    document.getElementById('f-name').value,
    email:   document.getElementById('f-email').value,
    phone:   document.getElementById('f-phone').value,
    message: document.getElementById('f-msg').value,
  };
  await fetch('https://formspree.io/f/YOUR_FORM_ID', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(data)
  });
  alert('Message sent! We will get back to you within 24 hours.');
}
```

---

## Design System

| Token | Value |
|-------|-------|
| Primary Font | Syne (800 weight headings) |
| Body Font | DM Sans (300–500 weight) |
| Background | `#0a0a0a` |
| Foreground | `#f5f2ee` |
| Accent (Gold) | `#c8a96e` |
| Border | `rgba(200,169,110,0.18)` |

---

## Services Offered

- Video Editing
- Motion Graphics
- 2D / 3D Animation
- Color Grading
- Sound Design
- Visual Effects

---

## Pricing Plans

| Plan | Price | Best For |
|------|-------|----------|
| Creator | $499/mo | Individual creators & small teams |
| Team | $1,199/mo | Growing brands & content teams |
| Studio | $2,499/mo | Production houses & agencies |

---

## Contact

- 🌐 Website: [dgcedits.com](https://dgcedits.com)
- 📧 Email: connect@dgcedits.com
- 📞 Phone: +91 79052 79486
- 📍 Location: Andheri West, Mumbai, India
- 🔗 LinkedIn: [DGC Film Works](https://www.linkedin.com/company/dgcfilmworks/)
- 📸 Instagram: [@dgc_edits](https://www.instagram.com/dgc_edits)
- 👍 Facebook: [dgcedits](https://www.facebook.com/dgcedits)

---

## License

© 2025 DGC Edits. All rights reserved. Powered by DGC Film Works.
