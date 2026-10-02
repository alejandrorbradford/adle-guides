# Adle guides

Public hosting for Adle's downloadable guides.

This repository exists so the files have a stable, direct URL that email
providers will fetch as an attachment. Brevo rejects attachment URLs on some
hosts (Wix's `usrfiles.com` among them) but accepts `raw.githubusercontent.com`.

| File | Pages | Language |
|---|---|---|
| `adle-anuncios-que-no-parecen-anuncios.pdf` | 24 | Spanish |
| `adle-ads-that-dont-look-like-ads.pdf` | 24 | English |

Both PDFs are page-image builds sized to fit Brevo's 4 MB ceiling on content
plus attachment, which is measured on the base64 encoding at roughly 1.33x the
file. The Spanish edition is a re-encode of the original design export
(11.5 MB down to 2.4 MB, 1100px pages). The English edition was rebuilt from
scratch in HTML and rendered at 1200px, 2.5 MB.

Link to a commit SHA rather than a branch: GitHub's raw CDN serves a stale file
for minutes after a push, and a branch URL would let an attachment change under
a campaign that already went out.
