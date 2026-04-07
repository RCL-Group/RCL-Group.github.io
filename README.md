# RCL Group Website

Official website of the **Robotics Cognition and Learning (RCL) Group**, led by Prof. Xingxing Zuo at the Robotics Department, MBZUAI (Abu Dhabi, UAE).

Built with [Hugo](https://gohugo.io/) and the [Hugo Blox](https://hugoblox.com/) academic theme.

**Live site:** https://RCL-Group.github.io/

---

## Quick Start (Local Development)

### Prerequisites

- [Hugo](https://gohugo.io/installation/) >= 0.152.1 (**extended version** required)
- [Go](https://golang.org/dl/) >= 1.21
- [Node.js](https://nodejs.org/) >= 22
- [pnpm](https://pnpm.io/installation) >= 10.14.0

### Run Locally

```bash
# Clone the repository
git clone https://github.com/RCL-Group/RCL-Group.github.io.git
cd RCL-Group.github.io

# Install dependencies
pnpm install

# Start local dev server with live reload
pnpm dev

# Open http://localhost:1313 in your browser
```

Any file edits will automatically reload in the browser.

### Build for Production

```bash
pnpm build    # Output in public/ directory
```

---

## Project Structure

```
RCL-Group.github.io/
├── config/_default/
│   ├── hugo.yaml          # Site title, base URL
│   ├── params.yaml        # Theme, SEO, header/footer
│   ├── menus.yaml         # Navigation menu
│   ├── languages.yaml     # Language settings
│   └── module.yaml        # Hugo module imports
├── content/
│   ├── _index.md          # ★ Homepage layout (all sections)
│   ├── authors/           # Team member profiles
│   │   ├── admin/         #   PI: Prof. Xingxing Zuo
│   │   ├── hongjia-zhai/  #   Postdoc
│   │   ├── huajian-zeng/  #   PhD Student
│   │   ├── yuantai-zhang/ #   PhD Student
│   │   ├── yasser-attia/  #   PhD Student
│   │   ├── chenru-wen/    #   M.Sc. Student
│   │   ├── jiaqi-yang/    #   Visiting PhD Student
│   │   ├── omar-garib/    #   Visiting Master Student
│   │   └── yiran-yuan/    #   Visiting Master Student
│   ├── publications/      # Publication entries
│   ├── blog/              # News posts
│   ├── research/          # Research area pages
│   ├── projects/          # Project pages (optional)
│   ├── events/            # Event pages (optional)
│   └── opportunities.md   # "Join Us" page
├── assets/media/          # Images, icons
├── static/                # Static files (PDFs, etc.)
└── public/                # Build output (gitignored)
```

---

## How to Edit the Website

### 1. Edit the Homepage

The homepage is defined in **`content/_index.md`**. It uses a block-based layout where each `- block:` entry is a section. You can edit text directly, reorder sections by moving blocks, or remove sections by deleting entire blocks.

### 2. Add a New Team Member

```bash
# 1. Create a folder with the member's name
mkdir content/authors/firstname-lastname

# 2. Create their profile
#    (copy an existing profile as a starting point)
cp content/authors/huajian-zeng/_index.md content/authors/firstname-lastname/_index.md

# 3. Edit the profile: update title, role, interests, education, social links
# 4. Add their photo as avatar.jpg (or .png) in the same folder

# 5. Set the correct user_groups in the frontmatter:
#    - Principal Investigators
#    - Postdoctoral Researchers
#    - PhD Students
#    - Research Assistants
#    - Visiting Students
```

### 3. Add a New Publication

```bash
# 1. Create a folder
mkdir content/publications/my-paper-2025

# 2. Create index.md with this format:
```

```yaml
---
title: 'Paper Title Here'
authors:
  - admin                    # Use folder names from content/authors/
  - huajian-zeng
date: '2025-06-01T00:00:00Z'
publication_types: ['paper-conference']  # or 'article-journal', 'preprint'
publication: 'In *ICRA 2025*'
publication_short: 'ICRA 2025'
abstract: 'Abstract text here.'
tags: ['SLAM', 'LiDAR']
featured: false
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/XXXX.XXXXX'
url_pdf: ''
url_code: ''
url_video: ''
---
```

### 4. Add a News Post

```bash
mkdir content/blog/my-news-item
```

Create `content/blog/my-news-item/index.md`:

```yaml
---
title: 'Paper Accepted at ICRA 2025!'
date: 2025-01-15
authors:
  - admin
tags:
  - Publication
---

Our paper "Paper Title" has been accepted at ICRA 2025!
```

### 5. Edit Research Areas

Research areas on the homepage are defined in `content/_index.md` under the `research-areas` block. Individual pages are in `content/research/`:

- `robot-perception.md` — Robot Perception & State Estimation
- `3d-vision.md` — 3D Vision & Spatial AI
- `embodied-ai.md` — Embodied AI & Human-Robot Interaction

### 6. Edit the "Join Us" Page

Edit `content/opportunities.md` to update positions and application instructions.

### 7. Edit Navigation Menu

Edit `config/_default/menus.yaml`. The `weight` field controls display order (lower = further left).

### 8. Edit Site Metadata

| What                    | File                          |
|-------------------------|-------------------------------|
| Site title & URL        | `config/_default/hugo.yaml`   |
| Theme, SEO, header      | `config/_default/params.yaml` |
| Navigation links        | `config/_default/menus.yaml`  |

### 9. Add Images

- Team photos: `content/authors/<name>/avatar.jpg`
- Publication images: `content/publications/<paper>/featured.jpg`
- General images: `assets/media/`

---

## Deployment

Pushing to `main` triggers automatic deployment via GitHub Actions (`.github/workflows/deploy.yml`). A Netlify config (`netlify.toml`) is also included as an alternative.

---

## Useful Links

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Hugo Blox Docs](https://docs.hugoblox.com/)
- [Hugo Blox Research Group Template](https://hugoblox.com/templates/details/research-group/)

---

## Commands

| Command        | Description                              |
|----------------|------------------------------------------|
| `pnpm install` | Install dependencies                     |
| `pnpm dev`     | Start dev server with hot reload         |
| `pnpm build`   | Build for production (output in `public/`)|
