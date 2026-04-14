# STR Webinar - Agent Instructions

## Project Overview
Webinar registration and confirmation pages for Preston Seo's Airbnb STR Workshop.

---

## Repository Information

**GitHub Repository**: https://github.com/LEGACY-INVESTING-SHOW/str-webinar

**Vercel Project**: https://vercel.com/legacy-investing-show/str-webinar

**Production URL**: https://str-webinar.vercel.app

**Custom Domain**: str.managemoney101.com (SSL pending)

---

## Deployment Instructions

### Prerequisites
- Must be authenticated with Vercel CLI (`vercel login`)
- Git must be configured with the correct author:
  ```bash
  git config user.name "preston-8034"
  git config user.email "preston@legacyinvestingshow.com"
  ```

### Deploy Process

1. **Make changes** to the files in `/Users/deveshdhardubey/Downloads/str webinar/`

2. **Stage and commit** with the correct author:
   ```bash
   cd "/Users/deveshdhardubey/Downloads/str webinar"
   git add <files>
   git commit -m "Your commit message"
   ```

3. **Push to GitHub**:
   ```bash
   git push origin main
   ```

4. **Deploy to Vercel**:
   ```bash
   vercel --prod --yes
   ```
   
   Or if already in the project directory:
   ```bash
   cd "/Users/deveshdhardubey/Downloads/str webinar" && vercel --prod --yes
   ```

### Important Notes

- **CRITICAL**: The git author MUST be `preston-8034` or Vercel will block the deployment
- Always deploy from the project directory, not home directory
- The project is already linked to `legacy-investing-show/str-webinar`
- Production deployments require the `--prod` flag

---

## File Structure

```
str webinar/
├── index.html                                 # Main registration page (root)
├── registered.html                            # Post-registration confirmation
├── preston fam rail.avif                      # Hero image
├── preston-family.webp                        # About section image
├── af204c7a353d959657f10645474ff2c1.webp     # Media logos
├── testimonial-01.png to testimonial-10.jpeg # Student testimonial images
├── vercel.json                                # Vercel configuration
└── .git/                                      # Git repository
```

---

## Tracking Scripts

Both HTML pages include:
- Google Tag Manager (GTM-KQ4R2LKP)
- LeadsTunnel universal tracking script

Do not remove these scripts - they are required for marketing attribution.

---

## Troubleshooting

### "Author not found" error
The git commit author must match the Vercel project owner. Fix with:
```bash
git config user.name "preston-8034"
git config user.email "preston@legacyinvestingshow.com"
git commit --amend --author="preston-8034 <preston@legacyinvestingshow.com>" --no-edit
git push --force-with-lease origin main
```

### "Unexpected error" during deploy
Ensure you're running the deploy command from the project directory:
```bash
cd "/Users/deveshdhardubey/Downloads/str webinar"
vercel --prod --yes
```

### Build fails
Check that all referenced images exist and are committed to git.
