# ClipLens AI — frontend starter

A responsive Next.js frontend inspired by the general workflow of online media utility websites.

## Included
- Responsive dark premium interface
- URL input and clipboard paste
- Basic client-side platform/domain recognition
- Output format and quality selectors
- Status and validation messages
- Feature, workflow, FAQ and footer sections

## Run locally
Requirements: Node.js 20.9+.

```bash
npm install
npm run dev
```

Open http://localhost:3000.

## Important: frontend prototype, not a live downloader
This project intentionally does not bypass platform restrictions or extract protected streams. The Continue button validates and recognizes the URL, then explains that a backend integration is needed.

To build production media processing:
1. Add a NestJS API with authenticated, rate-limited endpoints.
2. Support user-uploaded files and explicitly authorized direct media sources.
3. Validate URLs against SSRF, DNS rebinding, redirect and private-network risks.
4. Run FFmpeg in isolated workers with strict CPU, memory, duration and file-size limits.
5. Store outputs in private object storage and issue short-lived signed download URLs.
6. Add cleanup, audit logs, copyright/takedown handling and monitoring.

## Before launch
- Replace the demo name "Viora" with your brand.
- Replace the placeholder contact email.
- Add privacy policy, terms and copyright/takedown pages.
- Configure a real backend, storage and approved media integrations.
- Review applicable platform terms and local law.


## Cloudflare Pages deployment (static frontend)
- Framework preset: Next.js (Static HTML Export) or configure manually.
- Build command: `npm run build`
- Build output directory: `out`
- Node.js version: 20.9 or newer.
- This starter is frontend-only. It does not include a media-processing backend, FFmpeg workers, database, or admin dashboard.
