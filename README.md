# nyora-mihon-local

A single **fully-local** Mihon extension: bundles the kotatsu-parsers engine and
exposes ~900 sources that parse **on-device** — no server.

## Add in Mihon
Browse → Extensions → ⋮ → Extension repos → Add:

```
https://raw.githubusercontent.com/Hasan72341/nyora-mihon-local/main/index.min.json
```

Then install **Nyora (Local)** — one APK, all sources.

> HTTP/JSON/Jsoup sources work out of the box. Cloudflare/JS-protected sources
> need an on-device WebView (`evaluateJs`) which is not yet wired up.
