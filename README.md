# Posts

Static, self-contained HTML pages published with **GitHub Pages** to accompany
content shared on LinkedIn. Live at <https://lucasns97.github.io/Posts/>.

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

- **Agentes de IA: do texto à ação** — `posts/ai-agents/` — navigable
  presentation deck (pt-BR). Its slide 8 multi-agent demo links to the companion
  data page **Smartphone Access by Generation** (`smartphone-per-gen.html`).
