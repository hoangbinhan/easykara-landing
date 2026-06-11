# CLAUDE.md

@AGENTS.md

## Command

- `pnpm dev` — Astro dev server
- `pnpm build` — Build static site
- `pnpm preview` — Preview build
- `pnpm lint` — ESLint
- `pnpm format` — Prettier

## Architecture

- **Framework:** Astro (static output) + Cloudflare Pages adapter
- **Styling:** Tailwind CSS v4 — see DESIGN.md for tokens
- **React islands:** Interactive components only (demo widget, pricing toggle, etc.)
- **i18n:** `src/i18n/en.ts` / `vi.ts` — never hardcode strings in templates
- **Images:** Use `<Image>` from `astro:assets` for optimization

## Deploy

- Production: `easykara.com` via Cloudflare Pages
- Branch `main` → auto deploy

