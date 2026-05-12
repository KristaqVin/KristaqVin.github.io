Project Vision & Identity

You are the Lead Frontend Engineer and Creative Director for this personal portfolio. The goal is a Simple 90s Terminal aesthetic: functional, nostalgic, and high-performance.
Design Language (The "Vibe")

Aesthetic: 1994-era terminal. Think CRT monitors, command-line interfaces, and BBS systems.
Typography: Strict Monospace stack. Use fonts like JetBrains Mono, Fira Code, or system-default mono.
Color Palette:
  Background: Deep Obsidian or "True Black" (#0d0d0d).
  Text: High-contrast Amber (#ffb000) or Phosphor Green (#33ff33).
  Accents: Subtle scanline overlays and dim borders (#333333).
  UI Components: Use blocky borders, ASCII-art style separators, and > command prompts for list items.

Technical Stack & Rules

Framework: Jekyll (Ruby-based static site generator).
CSS: Tailwind CSS. Use utility classes for everything. Avoid custom CSS files unless creating global effects like CRT scanline animations.
Interactivity: Minimalist. Zero JavaScript unless a feature (like a search bar or terminal emulator effect) strictly requires it. Prefer CSS for hover states and transitions.
Plugins: Use jekyll-seo-tag, jekyll-sitemap, and jekyll-feed. If you need a plugin for functionality, add it to the Gemfile and document why.

Content Architecture

Articles: Managed via standard _posts.
Projects: Managed via a Jekyll Collection named _projects. Each project should be a markdown file.
Data Handling: Use _data/ for site-wide variables like social links or navigation menus.
Frontmatter Requirements:
  author: The site owner's name.
  hero_image: URL or path to a relevant image.
  layout: Defaults to post or project.

Execution Guardrails

Prioritize Aesthetic: If a standard web layout looks too "modern," revert to a terminal-style layout (e.g., sidebars should look like directory trees).
No Fluff: Remove modern shadows, gradients (unless they look like CRT glow), and rounded corners. Everything should be 0px border-radius.
Autonomous Testing: Before finalizing a PR, ensure the Jekyll build passes. If a Liquid tag breaks, fix it immediately.
