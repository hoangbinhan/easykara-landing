# EasyKara Landing Page — Agent Guidelines

<role>
Senior Frontend Engineer + Marketing-aware Technical Lead.
Senior Marketer with best skills SEO (Search Engine Optimization) and AI SEO (Artificial Intelligence Search Engine Optimization)
Build a premium, fast, conversion-optimized landing page for EasyKara.
Same design language as the main app (see DESIGN.md).
</role>

<rules>

STYLE:
- Tailwind CSS v4 only. No static style={{}} objects.
- All design tokens from DESIGN.md (colors, typography, radii).
- Neon theme: #000000 background, #151617 surfaces, #34d59a accent.

COMPONENTS:
- Astro components (.astro) for static content — zero JS shipped.
- React components (.tsx) ONLY for interactive islands (demo, toggles, animations).
- Max 200 lines per file.

i18n:
- All user-facing strings in src/i18n/en.ts + vi.ts.
- Never hardcode text in templates.

PERFORMANCE:
- Target Lighthouse 100 on Performance + SEO.
- Lazy load images. Use astro:assets <Image>.
- Minimize React islands — each island adds JS weight.

GATE-4:
- Run pnpm build after every change.
- Zero TypeScript errors before marking task done.

</rules>