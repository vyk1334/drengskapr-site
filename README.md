# Drengskapr Viking Spirit — Website

Static HTML/CSS/JS site for [Drengskapr Viking Spirit](https://www.drengskaprvikingspirit.com).

## Structure

```
/
├── index.html              # Homepage
├── store.html              # Store (returning soon)
├── calendar.html           # Heathen Calendar landing page
├── about.html              # About / The Code of the Drengr
├── contact.html            # Contact Us
├── heathen-calendar-v1.html  # The Heathen Lunisolar Calendar app
├── assets/
│   ├── style.css           # Shared styles
│   └── main.js             # Shared JS (nav, scroll reveal)
└── README.md
```

## Deployment

### GitHub Pages
1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your site will be live at `https://yourusername.github.io/repo-name`

### Custom Domain
1. Add a `CNAME` file to this folder containing your domain (e.g. `www.drengskaprvikingspirit.com`)
2. In your domain registrar's DNS settings, add a CNAME record:
   - Name: `www`
   - Value: `yourusername.github.io`
3. For the apex domain (`drengskaprvikingspirit.com`), add four A records pointing to GitHub's IPs:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`

### Netlify (Alternative — Recommended)
1. Drag and drop this folder into [app.netlify.com/drop](https://app.netlify.com/drop)
2. Or connect your GitHub repo in Netlify dashboard
3. Set your custom domain in **Domain Management**

## Contact Form
The contact form currently shows a success message client-side only. To make it actually send messages, replace the submit handler in `contact.html` with one of:
- **Formspree**: Add `action="https://formspree.io/f/YOUR_ID"` to the form tag
- **Netlify Forms**: Add `data-netlify="true"` to the form tag (auto-works on Netlify)
- **EmailJS**: Use the EmailJS SDK to send directly from the browser

## Notes
- No build step required — pure HTML/CSS/JS
- All social links are live and correct
- Copyright year auto-updates via JS
- `heathen-calendar-v1.html` is the standalone calendar app (self-contained)

## Copyright
© Drengskapr Viking Spirit, LLC. All Rights Reserved.
