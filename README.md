# FasterFold website

The marketing site for [FasterFold](https://www.youtube.com/@fasterfold-ai): agentic software today, robotics next.

**Build with AI. Ship with proof.**

## What's here

A single static page. No build step, no dependencies.

```
index.html     the whole site: markup, styles and script
assets/        logo, favicon and TokenTelemetry dashboard captures
```

Sections, in order: hero, proof points, what we build, products
([TokenTelemetry](https://tokentelemetry.com/), the Shorts Engine, embodied agents),
how we work, robotics roadmap, channel, FAQ and the project brief form.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 4173
```

Then visit http://localhost:4173.

## Things to edit

All of these are in `index.html`.

| What | Where |
| --- | --- |
| Address that project briefs are sent to | `CONTACT_EMAIL` at the top of the `<script>` block. It is empty until you set it. |
| Videos shown in the robotics and channel sections | The `ROBOTS` and `CHANNEL` lists (YouTube video ID, title, label) |
| Proof figures (agents, stars, video count) | The `proof` section. Update the "Figures as of" date with them. |
| Colours and fonts | The `:root` variables at the top of the `<style>` block |

## Notes

- The proof figures are a snapshot from November 10, 2026 and will go stale.
- Video thumbnails load from YouTube; everything else is local.
- The contact form opens the visitor's email app with the brief filled in. Nothing is stored or sent by the site itself.
- Fonts (Space Grotesk, Inter, IBM Plex Mono) load from Google Fonts.

## Deploy

Any static host works. For GitHub Pages: Settings → Pages → deploy from the `main` branch, root folder.
