# Joseph Elhoregy - Portfolio Website

A professional portfolio website for Joseph Elhoregy, Senior Technical Manager.

**Live URL:** [ellytech.io/about-joseph](https://ellytech.io/about-joseph)

---

## Quick Start

### 1. Add Your Profile Photo

Replace the placeholder with your actual photo:

```
about-joseph/assets/images/profile.jpg
```

**Requirements:**
- Square image recommended (at least 400x400 pixels)
- JPEG or PNG format
- Name it `profile.jpg`

### 2. Deploy to Cloudflare Pages

Since you have `ellytech.io` on Cloudflare:

1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com)
2. Select your account
3. Go to **Pages** > **Create a project**
4. Connect your GitHub repository
5. Set these build settings:
   - **Build command:** (leave empty - it's a static site)
   - **Build output directory:** `/` (root)
6. Click **Save and Deploy**

The site will be available at `ellytech.io/about-joseph`

---

## Editing Your Website

### File Structure

```
elly-website/
├── index.html                    # Redirects to /about-joseph
├── README.md                     # This file
└── about-joseph/
    ├── index.html                # Main portfolio page
    └── assets/
        ├── css/
        │   └── style.css         # All styling
        ├── js/
        │   └── main.js           # Interactivity
        └── images/
            └── profile.jpg       # YOUR PHOTO GOES HERE
```

### Editing Sections

All content is in `about-joseph/index.html`. Each section has clear comments:

#### Personal Information (Hero Section)
Look for: `<!-- HERO SECTION -->`

```html
<h1 class="hero-name">Joseph Elhoregy</h1>
<h2 class="hero-title">Senior Technical Manager</h2>
<p class="hero-description">Your summary here...</p>
```

#### About Section
Look for: `<!-- ABOUT SECTION -->`

Edit the text inside `<p>` tags and update the highlights (years, cases, equipment value).

#### Experience
Look for: `<!-- EXPERIENCE SECTION -->`

Each job is a `timeline-item`. To add a new job, copy an existing `timeline-item` and edit:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <div class="timeline-header">
            <div>
                <h3 class="job-title">Your Job Title</h3>
                <h4 class="company">Company Name</h4>
            </div>
            <div class="timeline-meta">
                <span class="location"><i class="fas fa-map-marker-alt"></i> Location</span>
                <span class="date"><i class="fas fa-calendar"></i> Start - End</span>
            </div>
        </div>
        <ul class="job-description">
            <li>Achievement 1</li>
            <li>Achievement 2</li>
        </ul>
    </div>
</div>
```

#### Certifications
Look for: `<!-- CERTIFICATIONS SECTION -->`

Each certification is a `cert-card`. Add more by copying:

```html
<div class="cert-card">
    <div class="cert-logo">
        <i class="fas fa-shield-alt"></i>
    </div>
    <h3 class="cert-name">Certification Name</h3>
    <p class="cert-issuer">Issuer</p>
    <p class="cert-date">Month Year</p>
</div>
```

#### Skills
Look for: `<!-- SKILLS SECTION -->`

Add skills as tags:

```html
<span class="skill-tag">New Skill</span>
```

#### Projects
Look for: `<!-- PROJECTS SECTION -->`

Each project is a `project-card`. Add links to your actual projects.

#### Contact Information
Look for: `<!-- CONTACT SECTION -->`

Update email, phone, and social links.

#### Social Links (Multiple Locations)
Update these in both the hero and contact sections:

```html
<a href="https://github.com/yourusername" class="social-link">
<a href="https://linkedin.com/in/yourprofile" class="social-link">
<a href="mailto:your@email.com" class="social-link">
```

---

## Customizing Colors

Edit the CSS variables at the top of `about-joseph/assets/css/style.css`:

```css
:root {
    /* Change these to customize your color scheme */
    --primary-color: #2563eb;      /* Main accent color */
    --primary-hover: #1d4ed8;      /* Hover state */
    --primary-light: #dbeafe;      /* Light background */
    --text-primary: #1e293b;       /* Main text */
    --text-secondary: #475569;     /* Secondary text */
}
```

**Popular Color Schemes:**

| Theme | Primary | Hover | Light |
|-------|---------|-------|-------|
| Blue (default) | `#2563eb` | `#1d4ed8` | `#dbeafe` |
| Green | `#10b981` | `#059669` | `#d1fae5` |
| Purple | `#8b5cf6` | `#7c3aed` | `#ede9fe` |
| Red | `#ef4444` | `#dc2626` | `#fee2e2` |
| Orange | `#f97316` | `#ea580c` | `#ffedd5` |

---

## Adding More Pages

To add a new page (e.g., `/about-joseph/blog/`):

1. Create folder: `about-joseph/blog/`
2. Create: `about-joseph/blog/index.html`
3. Copy the structure from the main page
4. Update navigation links

---

## Icons Reference

The site uses [Font Awesome 6](https://fontawesome.com/icons). Common icons:

- `fa-envelope` - Email
- `fa-phone` - Phone
- `fa-map-marker-alt` - Location
- `fa-github` - GitHub
- `fa-linkedin` - LinkedIn
- `fa-shield-alt` - Security
- `fa-network-wired` - Networking
- `fa-server` - Server/Infrastructure
- `fa-code` - Development
- `fa-graduation-cap` - Education

---

## Troubleshooting

**Image not showing?**
- Make sure the file is named exactly `profile.jpg`
- Check it's in `about-joseph/assets/images/`

**CSS not updating?**
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)

**Changes not appearing on live site?**
- Push changes to GitHub
- Cloudflare Pages will auto-redeploy (takes 1-2 minutes)

---

## Support

Need help? Here are some resources:

- [HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML)
- [CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/CSS)
- [Cloudflare Pages Docs](https://developers.cloudflare.com/pages/)
- [Font Awesome Icons](https://fontawesome.com/icons)
