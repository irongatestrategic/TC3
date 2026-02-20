# The Coffee Can Camp (TC3)

**thecoffeecancamp.com**

Gear advice from someone who learned the hard way. Stories from the trail. No fluff, no perfection — just what works.

## Stack

- [Eleventy](https://www.11ty.dev/) static site generator
- [Cloudflare Pages](https://pages.cloudflare.com/) for hosting
- Nunjucks templates
- Plain CSS — no frameworks

## Local Development

```bash
npm install
npm start
```

Site runs at `http://localhost:8080`

## Build

```bash
npm run build
```

Output goes to `_site/`

## Structure

```
src/
├── _data/         # Site-wide data (site.js)
├── _includes/
│   └── layouts/   # base.njk, post.njk, page.njk
├── assets/
│   └── css/       # style.css
├── posts/         # Blog posts (.md)
├── pages/         # Static pages (.md)
├── index.njk      # Homepage
├── stories.njk    # Stories index
└── feed.njk       # RSS feed
```

## Deployment

Push to GitHub → Cloudflare Pages auto-deploys.

Build command: `npm run build`
Output directory: `_site`

## The Origin Story

A church trip leader once handed Jeff a cast iron skillet to carry into the backcountry. He swore he'd never let anyone pick his gear again. This site is what happened next.
