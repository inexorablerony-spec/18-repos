# Added provider pack

Added source files under `providers/` and corresponding CommonJS files under `dist/` for:
- Eporner (`eporner`)
- Erome (`erome`)
- HQPorner (`hqporner`)
- TNAFlix (`tnaflix`)

The existing manifest entries were preserved. The four new entries are appended with
`disabled: true`.

IMPORTANT: These are conservative HTML-parser scaffolds, not verified site integrations.
Listing selectors are generic, and stream extraction only returns direct MP4/HLS URLs
already exposed in the fetched page HTML. They do not bypass login, age checks, CAPTCHA,
DRM, anti-bot protections, or embedded-player restrictions. Some or all sites may return
no results until their site-specific HTML/API behavior is tested and the parsers are adapted.
No claim of 4K support or successful playback is made.

The original repository files were otherwise left in place.
