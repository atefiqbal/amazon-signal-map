# Amazon Signal Map

Landing page for **The Amazon Signal Map** — a free playbook for Amazon sellers explaining the 5 behavioral signals Amazon tracks per search query.

Live: [amazon-signal-map.vercel.app](https://amazon-signal-map.vercel.app)

---

## Structure

```
index.html     — Landing page (self-contained, 37KB)
vercel.json    — Vercel routing + security headers
```

## Before going live

**One required step:**

Open `index.html` and find `DELIVERY_CONFIG` near the bottom of the `<script>` block. Set your LinkedIn profile URL:

```javascript
linkedInUrl: "https://www.linkedin.com/in/your-handle",
```

If left empty, the LinkedIn "Questions?" link simply won't appear in the confirmation state — everything else works.

## Delivery config

| Setting | Current value |
|---|---|
| `mode` | `notion` |
| `notionUrl` | Set ✅ |
| `linkedInUrl` | Empty — add your handle |

## Deployment

Auto-deploys on every push to `main` via Vercel.

Manual redeploy: `vercel --prod`

## Custom domain

Recommended: `amazonsignalmap.com`

Add via Vercel Dashboard → Project Settings → Domains.
