# وعد — preview site

Static one-page site (HTML + CSS + JS, no build step). Arabic, right-to-left.

## Deploy to Vercel

From this folder:

```
npx vercel          # first time: log in, accept defaults ("Other" framework, no build command)
npx vercel --prod   # publish to the production URL
```

Or push this folder to a GitHub repo and import it at vercel.com/new (Framework: Other, no build command, output = root).

## Before launch (this is a preview)

- The kosha photos are AI-made samples: replace `hero.jpg`, `hero-arch.jpg`, `pink.jpg`, `red.jpg`, `candles.jpg`, `neon.jpg`, `white.jpg`, `stage-1.jpg`, `stage-3.jpg` with Esraa's real photos (same names, landscape for hero/stage, portrait 4:5 for the others).
- Confirm the WhatsApp number (in the script: `wa.me/201115140807`) and the FAQ answers.
- Remove the two `noindex` lines (in `index.html` and `vercel.json`) when the real site goes live, so Google can find it.
- After the first deploy, change `og:image` in `index.html` to the full URL (`https://<your-site>.vercel.app/og.jpg`) so WhatsApp shows the preview picture reliably.
