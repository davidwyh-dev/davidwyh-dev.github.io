# Personal Portfolio - Built with Claude Code

A minimal, dark-mode portfolio website showcasing projects built with AI-assisted development tools.

## Quick Start

### Local Development

1. Install Jekyll (if not already installed):
   ```bash
   gem install bundler jekyll
   ```

2. Run the local server:
   ```bash
   bundle exec jekyll serve
   ```

3. Open `http://localhost:4000` in your browser

### Deploy to GitHub Pages

1. Create a new repository on GitHub named **`davidwyh-dev.github.io`**
   - This special naming gives you the root URL (no `/repo-name` suffix)
2. Push this code to that repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/davidwyh-dev/davidwyh-dev.github.io.git
   git push -u origin main
   ```
3. Go to **Settings** → **Pages**
4. Under "Build and deployment", select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**

Your site will be live at `https://davidwyh-dev.github.io/`

## Customization

### Update Your Information

- **`_config.yml`** - Site title, description, and author name
- **`index.md`** - Hero text, about section, skills, and contact links
- **`_data/projects.yml`** - Add or modify your projects

### Adding a New Project

Edit `_data/projects.yml` and add a new entry:

```yaml
- name: "Your Project Name"
  description: "Brief description of what it does"
  icon: "🎯"  # Any emoji
  tags:
    - Technology1
    - Technology2
  github: "https://github.com/username/repo"
  live: "https://your-live-demo.com"  # Optional
  featured: true
```

### Updating Contact Links

In `index.md`, find the contact section and replace:
- `https://github.com/yourusername` with your GitHub profile
- `https://linkedin.com/in/yourusername` with your LinkedIn profile
- `your.email@example.com` with your email address

## File Structure

```
├── _config.yml          # Jekyll configuration
├── _layouts/
│   └── default.html     # Main HTML template
├── _data/
│   └── projects.yml     # Project data
├── assets/
│   └── css/
│       └── main.css     # All styles
├── index.md             # Landing page content
└── README.md            # This file
```

## Tech Stack

- **Jekyll** - Static site generator
- **GitHub Pages** - Hosting
- **Vanilla CSS** - No frameworks, pure CSS
- **JetBrains Mono & Space Grotesk** - Typography

---

Built with [Claude Code](https://claude.com/claude-code) 🤖
