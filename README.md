# Market King — Strategic Marketing Engine

A single-file marketing strategy engine powered by Google Gemini and a built-in
library of **1,001 marketing tips** distilled from 12 strategic frameworks
(brand identity, audience personas, copywriting, competitive positioning,
channels, campaign metrics, digital strategy, market research, lead generation,
brand auditing, retention, and pricing).

Everything runs in one `index.html` file. No build step, no server, no backend.

## Features

- **5-state strategy engine** — Initialize → Research → Ideation → Playbook → Export
- Works for an **existing brand** or a **new / custom product** (studies analogous brands)
- **20 campaign ideas** in four strategic groups, with "add 5 more" on demand
- **Detailed playbooks** per idea (hook, persona, channel blueprint, visual guardrails, attribution)
- **Knowledge library** of 1,001 tips — search, filter, star, copy, and **apply any tip to your brand**
- **Projects** auto-saved locally; rename, duplicate, delete
- Export any output as **dark-themed HTML** or **Markdown**
- 3 user-labelled Gemini key slots with active-key-first rotation and auto-fallback

## Setup

1. Open the app (see hosting below, or just open `index.html` locally in a browser).
2. Go to **Settings** and paste a Google Gemini API key into one of the three slots.
   Get a free key at https://aistudio.google.com/apikey
3. That's it. Keys are stored only in your browser (localStorage) — they are never
   committed to this repo or sent anywhere except Google's API.

## Hosting on GitHub Pages (free)

Because no secrets are baked into the file, this repo can be **public** and use
free GitHub Pages:

1. Push this repo to GitHub (see the repo's own instructions / below).
2. On GitHub, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/ (root)**, then **Save**.
5. Wait ~1 minute. Your app will be live at:
   `https://<your-username>.github.io/<repo-name>/`

Each visitor enters their own Gemini key on their own device.

## Privacy / keys

- API keys live in the browser's localStorage on each user's device.
- Nothing is stored server-side; there is no server.
- Do **not** hard-code a key into `index.html` if the repo is public — anyone could read it.

## License

MIT — see [LICENSE](LICENSE).
