# OsArq — osarq.com

Portfolio site for OsArq (Os Arquitectura), a residential architecture studio led by John Osborne in Tamarindo, Costa Rica.

## Stack
- Static HTML/CSS/JS (no build step needed)
- Google Fonts (Cormorant Garamond)
- Cloudflare Pages for hosting

## Deploy: GitHub → Cloudflare Pages

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "initial site"
git remote add origin git@github.com:YOUR-USERNAME/osarq-site.git
git push -u origin main
```

If using **GitHub Codespaces** or **Termius** from iPad:
- Create the repo on github.com first
- Clone it in Codespaces
- Copy these files in, commit, push

### 2. Connect Cloudflare Pages
1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com) → Pages
2. Click **Create a project** → **Connect to Git**
3. Select your `osarq-site` repo
4. Settings:
   - **Build command:** (leave blank — no build needed)
   - **Build output directory:** `/` (root)
5. Deploy

### 3. Custom Domain
1. In Cloudflare Pages project → **Custom domains**
2. Add `osarq.com`
3. If domain is already on Cloudflare, DNS is automatic
4. If not, point your domain's nameservers to Cloudflare first

## Project Structure
```
osarq-site/
├── index.html          # Full site (single page)
├── images/
│   ├── hero.jpg                # Hero banner (curved timber roof)
│   ├── philosophy-exterior.jpg # Hillside house in forest
│   └── philosophy-interior.jpg # Interior living space
└── README.md
```

## To Do
- [ ] Replace project placeholder images with real photography
- [ ] Add John's portrait photo to Studio section
- [ ] Set up Google Business Profile
- [ ] Configure SEO (sitemap.xml, robots.txt)
- [ ] Add Google Analytics / Cloudflare Web Analytics
- [ ] Mobile hamburger menu
- [ ] Individual project pages (phase 2)

## Image Replacement
Swap any `images/*.jpg` with final photography. Recommended sizes:
- **hero.jpg**: 1400px wide, 60% quality JPEG
- **philosophy images**: 800–1200px wide, 55% quality
- **project photos**: 800px wide per card

## Notes
- Design based on Rob Mills + Takt Studio aesthetic
- Dark palette: `#0A0A0A` bg, `#E8E2D8` text, `#A0B08A` muted green accent
- Typography: Cormorant Garamond (serif) + Helvetica Neue (sans)
