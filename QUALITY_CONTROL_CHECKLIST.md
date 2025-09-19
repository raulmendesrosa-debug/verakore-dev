# Verakore Website Quality Control Checklist

## Pre-Deployment Checklist

### Code Review
- [ ] Cross-page scrolling fix present in `services.html`
- [ ] All HTML files have proper structure
- [ ] CSS files are properly linked
- [ ] All images have alt text
- [ ] No broken links or missing files
- [ ] Contact forms are properly configured
- [ ] Meta tags are present and correct

### Local Testing
- [ ] Start local server: `python -m http.server 8000`
- [ ] Test homepage loads: `http://localhost:8000`
- [ ] Test services page loads: `http://localhost:8000/services.html`
- [ ] Test cross-page navigation (Services → Home)
- [ ] Test all navigation links work
- [ ] Test responsive design on mobile/tablet
- [ ] Test all pages load without errors
- [ ] Verify images load correctly
- [ ] Check contact forms work

### File Structure Verification
- [ ] `dev` folder contains only necessary files
- [ ] `prod` folder contains only necessary files
- [ ] Both folders have identical content
- [ ] No development files in production folder
- [ ] Assets folder structure is correct

## Deployment Process

### Dev Environment (GitHub)
- [ ] Navigate to `dev` folder
- [ ] Check git status: `git status`
- [ ] Add changes: `git add .`
- [ ] Commit changes: `git commit -m "Description of changes"`
- [ ] Push to GitHub: `git push origin master`
- [ ] Verify GitHub repository updated
- [ ] Test GitHub Pages deployment (if enabled)

### Production Environment (Cloudflare)
- [ ] Copy tested files from `dev` to `prod`
- [ ] Verify `prod` folder has latest changes
- [ ] Upload `prod` folder to Cloudflare Pages
- [ ] Verify Cloudflare deployment successful
- [ ] Check Cloudflare Pages URL

## Post-Deployment Verification

### Live Site Testing
- [ ] Test homepage loads on live site
- [ ] Test services page loads on live site
- [ ] Test cross-page scrolling fix works
- [ ] Test all navigation links work
- [ ] Test responsive design on live site
- [ ] Test contact forms work
- [ ] Verify images load correctly
- [ ] Check page load speeds
- [ ] Test on different browsers
- [ ] Test on mobile devices

### Performance Check
- [ ] Page loads within 3 seconds
- [ ] Images are optimized
- [ ] CSS/JS files are minified (if applicable)
- [ ] No console errors in browser
- [ ] Mobile responsiveness works

### Security Check
- [ ] HTTPS is enabled
- [ ] Security headers are present
- [ ] No sensitive information exposed
- [ ] Contact forms are secure

## Rollback Plan
- [ ] Keep backup of previous version
- [ ] Know how to revert changes
- [ ] Have contact information for support
- [ ] Document any issues found

## Sign-off
- [ ] All checklist items completed
- [ ] Live site tested and working
- [ ] Cross-page scrolling fix verified
- [ ] Ready for production use

**Deployment Date:** ___________
**Deployed By:** ___________
**Tested By:** ___________
**Approved By:** ___________

---

## Quick Reference

### Common Commands
```bash
# Start local server
python -m http.server 8000

# Git commands
git status
git add .
git commit -m "Description"
git push origin master

# Test URLs
Local: http://localhost:8000
GitHub Pages: https://raulmendesrosa-debug.github.io/verakore-dev
Cloudflare: [Your Cloudflare Pages URL]
```

### Critical Files to Check
- `index.html` - Homepage
- `services.html` - Services page (with cross-page scrolling fix)
- `assets/css/styles.css` - Main stylesheet
- `assets/images/` - All images
- `_headers` - Security headers
- `netlify.toml` - Configuration

### Emergency Contacts
- **Technical Support:** [Your contact info]
- **Hosting Support:** Cloudflare Support
- **Domain Support:** [Your domain provider]

---

*This checklist should be completed for every deployment to ensure quality and consistency.*

