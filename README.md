# TokFlow — short-video social feed demo

A responsive React + Vite prototype inspired by short-form video platforms. It uses a dark interface, cyan/pink accents, a vertical snap feed, IntersectionObserver autoplay/pause, like/save/follow interactions, a comment drawer, share support, keyboard play/pause, and mobile navigation.

## Run locally

Requirements: Node.js 18+ and npm.

```bash
npm install
npm run dev
```

Open the local URL Vite prints. To make a production build:

```bash
npm run build
npm run preview
```

## Notes
- This is a front-end demo; accounts, server persistence, real uploads, moderation, and production authentication are not connected.
- The MP4s and avatars are externally hosted sample assets and need an internet connection. If a provider changes a URL or blocks hotlinking, replace the `video` URLs in `src/App.jsx` with your own licensed vertical MP4s.
- Some sample videos are landscape source footage and are cropped with `object-fit: cover` as a fallback.
- The feed's “Load more videos” button appends additional sample cards; a production version should use a paginated API or cursor-based infinite loading.
