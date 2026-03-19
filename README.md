# Benard Ndungu — Personal Portfolio
 
A modern, responsive personal portfolio website for **Benard Ndungu Mocha**, a software developer based in Kiambu, Kenya.
 
---
 
## 📁 Project Structure
 
```
portfolio/
├── index.html               # Main portfolio file (all HTML, CSS, JS in one file)
├── image.jpg                # Your profile photo (place in the same folder)
├── CURRICULUM VITAE.docx    # Your CV (linked for download)
└── README.md                # This file
```
 
---
 
## 🚀 Getting Started
 
### Option 1 — Open Directly in Browser
Since this is a pure HTML/CSS/JS project with no build steps, you can simply:
1. Place all files (`index.html`, `image.jpg`, `CURRICULUM VITAE.docx`) in the **same folder**
2. Double-click `index.html` — it opens straight in your browser
 
### Option 2 — Run with a Local Server (Recommended)
For the best experience (avoids any browser file-loading restrictions):
 
**Using VS Code Live Server:**
1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Right-click `index.html` → **Open with Live Server**
 
**Using Python:**
```bash
# Python 3
python -m http.server 8000
# Then open http://localhost:8000 in your browser
```
 
**Using Node.js:**
```bash
npx serve .
```
 
---
 
## ✏️ How to Customise
 
### 1. Profile Photo
Replace `image.jpg` in the project folder with your own photo.
- Keep the filename as `image.jpg`, **or** update the `src` attribute in `index.html`:
```html
<img src="YOUR_PHOTO.jpg" alt="Benard Ndungu" class="hero-avatar" ...>
```
- If no image is found, the page automatically shows your initials **"BN"** as a fallback.
 
### 2. CV Download
Replace `CURRICULUM VITAE.docx` with your latest CV file.
- If you rename the file, update both download links in `index.html`:
```html
<a href="YOUR_CV_FILENAME.docx" download="BenardNdungu_CV.docx" ...>
```
 
### 3. Personal Details
All your details are written directly in `index.html`. Search for and update:
 
| What to change | Where to find it |
|---|---|
| Name / tagline | Hero section `<h1>` and `<p>` tags |
| About Me text | `#about` section |
| Skills & tags | `#skills` section — edit the `<span class="tag">` elements |
| Education entries | `#education` section |
| Project names, descriptions, GitHub links | `#projects` section |
| Email address | `#contact` section — both the `href` and display text |
| Phone number | `#contact` section |
| GitHub profile URL | Contact section + footer social link |
| LinkedIn profile URL | Contact section social card |
 
### 4. Colors & Fonts
All design tokens are defined as CSS variables at the top of the `<style>` block:
```css
:root {
    --green: #00E676;        /* Primary accent color */
    --ink: #080D0A;          /* Page background */
    --surface: #0E1512;      /* Card/section background */
    --text: #E8F0EC;         /* Primary text */
    --text-muted: #7A9487;   /* Secondary text */
    ...
}
```
Change `--green` to any hex color to instantly retheme the entire site.
 
---
 
## 🌐 Deploying Online (Free Options)
 
### GitHub Pages (Recommended)
1. Create a GitHub repository named `yourusername.github.io`
2. Upload `index.html`, `image.jpg`, and `CURRICULUM VITAE.docx` to the repo
3. Go to **Settings → Pages → Source → main branch**
4. Your site will be live at `https://yourusername.github.io`
 
### Netlify
1. Go to [netlify.com](https://netlify.com) and sign up for free
2. Drag and drop your project folder onto the Netlify dashboard
3. Your site is instantly live with a public URL
 
### Vercel
1. Go to [vercel.com](https://vercel.com) and sign in with GitHub
2. Import your repository and deploy — no configuration needed
 
---
 
## 📦 Dependencies (All via CDN — no installation needed)
 
| Library | Purpose | Version |
|---|---|---|
| [Font Awesome](https://fontawesome.com) | Icons | 6.5.1 |
| [Google Fonts — Syne](https://fonts.google.com/specimen/Syne) | Display / headings font | Latest |
| [Google Fonts — DM Sans](https://fonts.google.com/specimen/DM+Sans) | Body text font | Latest |
 
All dependencies load from CDN. **No npm, no build tools, no frameworks required.**
 
---
 
## ✅ Features
 
- ⚡ Single-file HTML — zero dependencies to install
- 📱 Fully responsive — works on mobile, tablet, and desktop
- 🎨 Custom animated cursor (desktop)
- 🔄 Scroll progress bar
- 🟢 Fade-in animations on scroll (Intersection Observer API)
- 🧭 Sticky navigation with blur/glass effect
- 🌑 Dark theme with green accent
- 🖼️ Profile photo with graceful fallback to initials
- 📥 CV download button in nav and contact section
- 🔗 Direct contact links (email, phone, GitHub, LinkedIn)
 
---
 
## 📬 Contact
 
**Benard Ndungu Mocha**
- 📧 [benardndungu45@gmail.com](mailto:benardndungu45@gmail.com)
- 📞 +254 790 863 446
- 🐙 [github.com/Benard-ndungu](https://github.com/Benard-ndungu)
- 💼 [linkedin.com/in/benard-mocha-214650382](https://www.linkedin.com/in/benard-mocha-214650382/)
- 📍 Kiambu, Kenya
 
---
 
*Built with pure HTML, CSS & JavaScript — no frameworks, no fuss.*