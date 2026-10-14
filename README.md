# Curate legal pages

Static Curate landing, privacy, terms and support pages, with Vercel redirects to the corresponding Novas Agency routes.

## Files

- [index.html](index.html): retained landing page.
- [legal/curate/privacy/](legal/curate/privacy/), [legal/curate/terms/](legal/curate/terms/) and [legal/curate/help/](legal/curate/help/): retained static pages.
- [assets/](assets/): local app artwork.
- [vercel.json](vercel.json): the hosted redirect map, including the legacy `/CurateApp` route.

## Local review

There is no package manifest or build step. From this folder, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open `http://127.0.0.1:8000/`. This serves the retained HTML; Python's server does not apply Vercel redirects. Review hosted routing separately when a release is authorised. A local preview is not legal-content approval.
