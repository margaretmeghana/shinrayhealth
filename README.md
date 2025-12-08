# Shinray Health — Static Website

This repository is a plain static site (HTML / CSS / images). I organized files into the recommended layout:

Root files:
- index.html
- for-employers.html
- for-employees.html
- solutions.html
- contact.html
- about.html (placeholder)
- request-demo.html (placeholder)
- blog.html (placeholder)
- privacy-policy.html (placeholder)
- terms.html (placeholder)

Folders:
- css/style.css      (styles)
- images/*           (png/jpg/svg files)
- icons/*            (svg icons)

Important files:
- .nojekyll          (empty file so GitHub Pages doesn't run Jekyll)

How to move your current files into this structure (commands)
1. From your project root run:
   mkdir -p css images icons
   git mv style.css css/style.css

   # move images (adjust filenames as needed)
   git mv shinray_logo.png shinray_logo_white.png hero-diverse-team.jpg employer-focus.jpg employee-focus.jpg client-logo-1.png client-logo-2.png client-logo-3.png images/

   # move icons (adjust filenames as needed)
   git mv icon-24-7.svg icon-expert.svg icon-secure.svg icon-mental-wellness.svg icon-financial-eap.svg icon-physical-health.svg icon-leadership.svg icons/

2. Add the new files (if you copied them from this template), then:
   git add .
   git commit -m "Organize project: css/, images/, icons/ and add placeholders"
   git push origin main

Local preview:
- Python: python -m http.server 8000
  Open http://localhost:8000

Publish with GitHub Pages:
1. Push the repo to GitHub (branch `main`).
2. In the repository on GitHub go to Settings → Pages.
3. Under "Source" choose Branch: `main` and Folder: `/ (root)`.
4. Save. Wait a minute — your site will be available at:
   https://<your-github-username>.github.io/<repo-name>/

Notes & next steps:
- Replace placeholder content with your real copy.
- Verify all image/icon filenames match the paths in HTML.
- Keep paths relative (no leading slash) so the site works at /<repo-name>/.
- If you'd like, I can:
  - create the git commits and push changes if you give me the repo URL and permission, or
  - produce a simple GitHub Actions workflow to publish to gh-pages instead of using the root branch.