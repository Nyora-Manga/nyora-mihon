# nyora-mihon

The **Nyora** extension repo for [Mihon](https://mihon.app) / Tachiyomi. Fully local:
it bundles the native kotatsu-parsers engine and parses **on-device** — no server —
exposing hundreds of manga sources.

## Add to Mihon

**More → Settings → Browse → Extension repos → +** and paste:

```
https://raw.githubusercontent.com/Nyora-Manga/nyora-mihon/main/index.min.json
```

Then open **Browse → Extensions** and install:

| Extension | contents |
|---|---|
| **Nyora-Sources** | SFW sources |
| **Nyora-Sources 18+** | adult sources |

Installed **from this repo**, they **auto-trust** (Mihon matches the APK signature
against this repo's signing fingerprint). A sideloaded APK instead shows
*UNTRUSTED* — tap the shield → **Trust** once.

## Notes

- HTTP / JSON / Jsoup sources work out of the box; images descramble on-device.
- Cloudflare-protected sources use Mihon's built-in WebView solver — for a source
  stuck on a challenge, use **Open in WebView** to solve it, then retry.
- Updating from a **lower** version code? Mihon won't auto-update a downgrade —
  uninstall the old extension and reinstall from the repo.

## Contents

```
index.min.json   extension index Mihon reads
repo.json        repo metadata + signing fingerprint (auto-trust)
apk/             the two extension APKs
icon/            store icons
```

> Published automatically by CI — do not edit by hand. Source & build pipeline:
> [`Nyora-Manga/nyora-mihon-extension-porter`](https://github.com/Nyora-Manga/nyora-mihon-extension-porter).
