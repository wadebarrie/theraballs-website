# Theraballs Landing Page

Simple static "Coming soon" page for theraballs.com.

## Local development

```bash
python3 -m http.server 5173 --bind 127.0.0.1
# Open http://127.0.0.1:5173
```

## Deploy to Netlify (from GitHub)
1. Push this repo to GitHub (main branch).
2. In Netlify: New site from Git → GitHub → choose repo.
3. Build settings: Build command: none, Publish directory: "." (root).
4. Deploy. Netlify will auto-build on every push to main.

### Custom domain
- Add your domain in Netlify → Domains → Add custom domain → theraballs.com
- Either:
  - Use Netlify DNS (recommended): point nameservers to Netlify's (shown in UI); or
  - Keep current DNS and add records:
    - A @ → 75.2.60.5
    - A @ → 99.83.190.102
    - CNAME www → your-site-name.netlify.app

## License
MIT
