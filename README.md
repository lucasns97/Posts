# Posts

Static, self-contained HTML pages published with **GitHub Pages** to accompany
content shared on LinkedIn. Live at [lucasns97.github.io/Posts](https://lucasns97.github.io/Posts/).

## GitHub Pages deploy

This repository is a **project page**, so the public URL is:

- `https://lucasns97.github.io/Posts/`

The root URL `https://lucasns97.github.io/` belongs to the user site repository
(`lucasns97.github.io`) and does not serve this project directly.

Deployment is automated by GitHub Actions via `.github/workflows/deploy-pages.yml`
on every push to `main`.

## Structure

```
.
├── index.html              # Landing page — lists every post (edit when adding one)
└── posts/
    └── ai-agents/          # One folder per post (kebab-case slug)
        ├── index.html      # The post itself → served at /Posts/posts/ai-agents/
        └── smartphone-per-gen.html   # Companion/asset pages live beside the post
```

## Adding a new post

1. Create `posts/<slug>/index.html`.
2. Keep everything self-contained (inline CSS/JS, CDN libraries are fine) so the
   page works on its own when shared.
3. Add a card linking to it in the root `index.html`.

## Current posts

- **AI Agents: from text to action / Agentes de IA: do texto à ação** —
  `posts/ai-agents/` — navigable presentation deck with an in-page **EN/PT**
  language toggle. Its slide 8 multi-agent demo links to the companion data page
  **Smartphone Access by Generation** (`smartphone-per-gen.html`).
