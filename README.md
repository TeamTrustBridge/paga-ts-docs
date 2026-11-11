# paga-ts-docs

Unofficial documentation website for the [`paga-ts`](https://github.com/TeamTrustBridge/paga-ts) SDK for the
[Paga Engine API](https://developer-docs.paga.com/).

> **This is unofficial documentation.** It is not built, endorsed, supported or
> published by Paga. It is community-maintained and follows Paga's published API
> reference. Paga's own documentation is the source of truth — if these pages
> and Paga's disagree, Paga's is right.

## Site

<https://teamtrustbridge.github.io/paga-ts-docs/>

## How it is built

The site is plain HTML, CSS and JavaScript — no framework, no build step and
no runtime dependencies. Every page is fully readable with JavaScript
disabled; the script only adds a theme toggle, the mobile navigation, a filter
over the operation reference, and copy-to-clipboard buttons.

The content comes from a shared dataset in
[TeamTrustBridge/paga](https://github.com/TeamTrustBridge/paga), so this site
and the other two always describe the same operations.

- `docs/` — the generated site, committed so the repository is the fallback
- `docs/operations.json` — the dataset, machine-readable
- `docs/llms.txt` — a plain-text outline of the whole site
- `docs/sitemap.xml` — the page list

## Local preview

```bash
python3 -m http.server --directory docs 8000
```

## License

GPL-3.0 — see [LICENSE](LICENSE).
