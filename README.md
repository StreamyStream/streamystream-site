# StreamyStream callback site

A tiny, dependency-free static site providing a stable HTTPS redirect location required for Trakt developer-app registration.

- Base URL: https://streamystream.github.io/streamystream-site/
- Trakt redirect URI: https://streamystream.github.io/streamystream-site/trakt-callback/
- GitHub Pages source: `main`, `/(root)`, HTTPS enforced. No custom domain.

## Files

- `index.html`: landing page.
- `trakt-callback/index.html`: static registration placeholder.
- `.nojekyll`: disables Jekyll processing.
- `README.md`: this documentation.

## Scope and behavior

The completion message is static. This page does not validate or complete authorization. Neither page contains JavaScript, reads URL query parameters, processes tokens, submits forms, sends application data, uses analytics, sets cookies, or loads external assets. Styling is inline. A restrictive content security policy blocks scripts, external resources, and form submission; the referrer policy is `no-referrer`.

StreamyStream users will not log into Trakt. This repository implements no account sync or metadata integration. Trakt is intended only as a replaceable metadata/artwork provider in a separate future task. Playback, watch history, Continue Watching, progress, resume, and device handoff remain StreamyStream-owned.

No API keys, Trakt client identifiers, credentials, product source code, dependencies, or build system belong in this repository. The four website files were authored independently in this separate working folder.
