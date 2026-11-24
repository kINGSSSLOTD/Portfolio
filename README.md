# Yuraiba Oni — Portfolio

React + TypeScript + Tailwind CSS + Framer Motion + Lucide.

## Run

```bash
npm install
npm run dev      # http://localhost:5173
npm run build    # production build in /dist
```

## Make it yours

| What | Where |
| --- | --- |
| Email, social links, services, default tools | `src/data/site.ts` |
| Portfolio projects | `src/data/projects.ts` |
| Your portrait | save as `public/portrait.jpg` (appears automatically) |
| Your images / videos | put in `public/work/` and point `image` / `video` at them |

### Replacing reference work with your own
Each project has an `ownership` field:
- `reference`: someone else's work, shown with a **Reference** badge and attribution (`source`). Fill in `source.creator` and `source.url` for each.
- `own`: your work. Change `ownership` to `'own'` and delete `source`.
- `placeholder`: empty slot for categories you have no work in yet.

The 15 images you supplied are in `public/work/` and are currently marked as **reference** with "creator not yet credited". Please add the real creators (or mark them `own` if they are yours).

### Tools section
Click **Edit tools** on the page to add/remove tools and categories (saved in that browser's localStorage). For permanent changes, edit `defaultTools` in `src/data/site.ts`.

### Contact form
There is no backend. Submitting opens the visitor's email app with the message prefilled. To use Formspree/Web3Forms instead, replace the `mailto:` line in `src/components/Contact.tsx`.
