# Mate Creations — showcase site

Showcase for the **Yerba Mate** (dark) and **Tererê** (light) theme family and the
design system behind them: DTCG tokens compiled with Style Dictionary, WCAG
contrast checked in both themes.

Live: https://harbefas.github.io/matecreations-site/

Moved out of `harbefas.github.io` in September 2026, history intact — that
domain now hosts the Harbefas site.

## Stack

React 19 · Vite · Tailwind · GSAP.

## Commands

| Command              | Action                                              |
| :------------------- | :-------------------------------------------------- |
| `npm install`        | Install dependencies                                 |
| `npm run dev`        | Dev server                                           |
| `npm run build`      | Build to `./dist/`                                   |
| `npm run sync:tokens`| Re-vendor tokens from a local `mateCreations` checkout |

`sync:tokens` needs `~/code/personal/mateCreations` (override with
`MATECREATIONS=`). It is a local, manual step: the generated
`src/styles/mate-tokens.css` and `src/theme/tokens.generated.ts` are committed,
so CI builds without it.
