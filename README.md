# The Final Edition — Breaking News Farewell

A private, single-page noir newspaper experience built as a six-page interactive late edition about a mutual breakup: no scandal, no villain, no rewriting what mattered.

## Deploy to Vercel

This project is intentionally static: no build step and no dependencies.

1. Create a new GitHub repository.
2. Upload the files in this folder to the repository root.
3. In Vercel, choose **Add New → Project**, import the repository, and deploy.
4. Framework preset can stay **Other**. Build Command and Output Directory should stay blank.

Vercel serves `index.html` directly.

## Files

- `index.html` — complete experience (HTML/CSS/JS in one file)
- `subject-cover.png` — refreshed cover crop from the supplied photo
- `subject-detail.png` — archive/detail crop from the supplied photo
- `subject-night.png` — alternate archive crop from the supplied photo
- `theme.mp3` — original soundtrack, unchanged
- `vercel.json` — static hosting/security headers

## Controls

- Tap **Read the Late Edition** to enter and start audio.
- Swipe horizontally on mobile, use arrow buttons, or use keyboard arrow keys.
- Use the music button in the top-right to mute/unmute.
- Reduced-motion preferences are respected.

## Privacy

The page includes `noindex,nofollow,noarchive` because it is intended for one person. Remove that robots meta tag only if you deliberately want search engines to index it.

## Mobile / desktop

The existing mobile-first renderer is preserved. Phones show one paper page at a time with internal vertical scrolling when needed; wider screens show a two-page newspaper spread. Safe-area insets, `visualViewport`, short landscape phones, browser chrome changes, and vertical-vs-horizontal swipe detection remain enabled.

The photo assets were refreshed into local files so the deployed site does not depend on an old external image link.
