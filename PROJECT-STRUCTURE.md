# Hustomten Danderyd - Project Structure

## 📁 Repository: n3ovision/hustomten-danderyd

### Current Deployment Setup (2026-02-01)

**Vercel Deployment:**
- Deployed from: **Root directory** (main branch)
- HTML files are served directly from root
- Images are in `/images/` subdirectory

### Directory Structure

```
/
├── index.html              # Homepage (modern Tailwind design)
├── finsnickeri.html        # Finsnickeri service page
├── mobelrenovering.html    # Furniture renovation page
├── utomhusjobb.html        # Outdoor work page
├── tjanster.html           # Services overview
├── kontakt.html            # Contact page
├── om-mig.html             # About page
│
├── images/                 # All images
│   ├── logo.png
│   ├── logo-white.png
│   ├── finsnickeri.jpg
│   ├── utomhusjobb.jpg
│   ├── furniture-*.jpg
│   ├── outdoor-*.jpg
│   ├── partner-*.jpg/png
│   └── ...
│
├── modern-tailwind/        # LEGACY: Original development directory
│   └── (identical to root, kept for reference)
│
├── variant1/               # LEGACY: Old design variant
├── variant2/               # LEGACY: Old design variant
├── variant2-modern/        # LEGACY: Old design variant
│
├── vercel.json            # Vercel configuration
├── README.md              # Project readme
└── .git/                  # Git repository
```

## 🎨 Design System

**Framework:** TailwindCSS 3.x (via CDN)
**Color Scheme:**
- Primary: Blue/teal (#3b82f6, #06b6d4)
- Background: White/light gray
- Accent: Gold for highlights

**Typography:**
- Headings: Bold, large
- Body: Clean, readable
- Mobile-responsive

## 📝 Content Source

**Original site:** https://hustomten-sthlm.se
- All content scraped and modernized
- Images downloaded and optimized
- Structure adapted for modern Tailwind design

## 🚀 Deployment Workflow

### Current Setup (GitHub Auto-Deploy)
1. Push to `main` branch
2. GitHub triggers Vercel webhook
3. Vercel builds and deploys from root
4. Live at: https://hustomten-danderyd.vercel.app

### Manual Deployment (if needed)
```bash
cd /root/clawd/projects/hustomten
git add .
git commit -m "Update content"
git push origin main
# Vercel auto-deploys
```

## 🔄 Future Expansion Notes

### To Add New Pages:
1. Create new `.html` file in root directory
2. Follow existing Tailwind structure from `index.html`
3. Add images to `/images/` if needed
4. Update navigation in all pages
5. Commit and push to trigger deployment

### To Update Existing Pages:
1. Edit HTML files directly in root
2. Maintain Tailwind CDN approach (or migrate to build process)
3. Test locally if needed
4. Commit and push

### Recommended Next Steps:
- [ ] Migrate to Vite/Next.js for build optimization
- [ ] Add contact form backend integration
- [ ] Implement image optimization
- [ ] Add analytics
- [ ] SEO meta tags optimization
- [ ] Add sitemap.xml

## 🛠 Technical Stack

- **Frontend:** Static HTML + TailwindCSS
- **Hosting:** Vercel
- **Repository:** GitHub (n3ovision org)
- **CI/CD:** GitHub → Vercel auto-deploy
- **Images:** Self-hosted in `/images/`

## 📞 Key URLs

- **Live Site:** https://hustomten-danderyd.vercel.app
- **GitHub Repo:** https://github.com/n3ovision/hustomten-danderyd
- **Vercel Project:** https://vercel.com/n3ovisions-projects/hustomten-danderyd
- **Original Site:** https://hustomten-sthlm.se

---

**Last Updated:** 2026-02-01  
**Maintained by:** N3ovision + Clawdbot AI Assistant
