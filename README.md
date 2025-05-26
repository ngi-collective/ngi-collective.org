# NGI Collective Website 🤖

The NextGen Inventors Collective website built with Eleventy (a static site generator).

## 🚀 Quick Start

### First Time Setup
1. **Download the code**: Clone this repository to your computer
2. **Install tools**: Run `npm install` in your terminal
3. **Start coding**: Run `npm run dev` to see your changes live!

### Daily Development
- **See your changes**: `npm run dev` - Opens a local server at `http://localhost:8080`
- **Build for production**: `npm run build` - Creates final files in the `docs/` folder

## 📁 File Structure

```
├── index.html          # Home page
├── team.html          # Teams page  
├── sponsorship.html   # Sponsorship page
├── header.html        # Navigation menu (shared across pages)
├── footer.html        # Footer (shared across pages)
├── head.html          # CSS styles and page setup
└── docs/              # Built website files (auto-generated)
```

## ✏️ Making Changes

### Adding New Pages
1. Create a new `.html` file (like `contact.html`)
2. Start with this template:
```html
<!doctype html>
<html>
{% include "head.html" %}
<body class="page-wrapper">
{% include "header.html" %}

<!-- Your page content here -->

{% include "footer.html" %}
</html>
```
3. Add the page link to `header.html` navigation

### Editing Styles
- All CSS is in `head.html` between the `<style>` tags
- Look for existing classes like `.hero`, `.content`, `.btn` before creating new ones

### Updating Team Info
- Edit team details in `team.html`
- Update team achievements, member counts, etc.

## 🔧 Commands Explained

- `npm run dev` = Start development server with live reload
- `npm run build` = Build final website files for deployment
- `npm install` = Download required tools (only needed once)

## 🌐 Deployment

The website auto-deploys to GitHub Pages when you push changes to the main branch. Built files go to the `docs/` folder which GitHub serves as the live website.

## 💡 Tips for New Developers

- **Test locally first**: Always run `npm run dev` to check your changes
- **Save often**: The dev server automatically refreshes when you save files
- **Check the console**: Open browser dev tools (F12) to see any errors
- **Start small**: Make one change at a time and test it
