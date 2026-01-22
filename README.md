# Personal Portfolio - Built with Cursor

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

1. Push this repository to GitHub
2. Go to **Settings** → **Pages**
3. Under "Build and deployment", select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**

Your site will be live at `https://[username].github.io/[repo-name]/`

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

Built with [Cursor](https://cursor.sh) 🤖
