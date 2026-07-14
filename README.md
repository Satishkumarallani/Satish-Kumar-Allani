# Satish Kumar Allani — Portfolio

Personal portfolio site. Static HTML/CSS with no build step, no dependencies, no framework.

**Live:** _(add URL once deployed)_

## Structure

```
index.html    the entire site (styles + scroll-reveal JS inlined)
_headers      Cloudflare Pages security + cache headers
assets/       résumé PDF, book cover
```

## Local preview

```sh
python3 -m http.server 4321
```

Then open http://localhost:4321.

## Deploying (Cloudflare Pages)

Connect this repo in the Cloudflare dashboard:

- **Build command:** _(none)_
- **Build output directory:** `/`

Every push to `main` redeploys.

## Editing

Everything lives in `index.html`. Sections are commented (`<!-- hero -->`, `<!-- experience -->`,
`<!-- research & publications -->`, …).

Items marked `<!-- TODO -->` are publications awaiting a public link:

- **AI-Augmented Patch Prioritization** (ISACA) — needs article URL or PDF
- **The Global Ransomware Epidemic** (IJCISIM) — needs link or PDF
- **The Metamorphosis of Access** (IEEE SmartNets 2026, accepted) — add IEEE Xplore link once indexed
- **CyberFuse-CL** (ICETCI 2026) — currently marked *under review*; promote to accepted once the decision lands

To host a paper PDF, drop it in `assets/` and link it from that publication's `.pub-links` block.
