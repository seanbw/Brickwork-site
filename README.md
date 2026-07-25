# BrickWork Website

A multi-page static website converted from a Word brick-pattern template.  
Styled with the original red/crimson colour palette and Quicksand body font.

## 📁 File Structure

```
website/
├── index.html          # Home page
├── about.html          # About page
├── services.html       # Services page
├── contact.html        # Contact page
├── css/
│   └── style.css       # All styles (variables, layout, components)
├── js/
│   └── main.js         # Nav toggle, scroll reveal, stat counters, form
├── images/             # Drop your images here
├── .gitignore
└── README.md
```

## 🎨 Design System

| Token | Value |
|---|---|
| Primary Red | `#CE1628` |
| Dark Red | `#8B010E` |
| Mid Red | `#B10F1F` |
| Orange Red | `#DB2F03` |
| Gold Accent | `#FFBA06` |
| Body Font | Quicksand (Google Fonts) |
| Heading Font | Bahnschrift SemiBold |

## 🚀 GitHub Desktop → Cloudflare Pages

### Step 1 — Push to GitHub
1. Open **GitHub Desktop**
2. Click **File → Add Local Repository**
3. Browse to this `website/` folder → click **Add Repository**
   - If prompted "not a git repo", click **Create Repository**
4. Write a commit message (e.g. `Initial commit`) → click **Commit to main**
5. Click **Publish repository** (set to Public if using Cloudflare free tier)

### Step 2 — Deploy on Cloudflare Pages
1. Go to [dash.cloudflare.com](https://dash.cloudflare.com) → **Workers & Pages**
2. Click **Create application → Pages → Connect to Git**
3. Authorise GitHub and select your repository
4. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave blank)*
   - **Build output directory:** `/` *(or leave blank)*
5. Click **Save and Deploy**

Cloudflare will give you a `*.pages.dev` URL instantly.  
Every `git push` from GitHub Desktop will auto-redeploy. ✅

## ✏️ Customisation Checklist

- [ ] Replace `BrickWork` name/logo with your brand
- [ ] Update colours in `css/style.css` `:root` variables
- [ ] Add real images to `images/` and update `img-placeholder` divs
- [ ] Update contact details (email, phone, address) in all 4 HTML files
- [ ] Add your Google Maps embed in `contact.html`
- [ ] Connect contact form to a service (Formspree, Netlify Forms, etc.)
- [ ] Update `<title>` tags and add meta descriptions for SEO
- [ ] Add a real favicon

## 📬 Contact Form Options (free)

- **[Formspree](https://formspree.io)** — add `action="https://formspree.io/f/YOUR_ID"` to `<form>`
- **[Web3Forms](https://web3forms.com)** — similar, no backend needed
- **Cloudflare Pages Functions** — serverless function in the same repo