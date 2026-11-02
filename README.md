# devrig.dev website

Prebuilt static files captured from https://devrig.dev/ on 2 November 2026.
Published product version: **0.102**.

The 42 website content files are copied unchanged from the downloaded archive
`devrig.dev-published-0.102-2026-11-02.tar.gz` (SHA-256 `0141d8c07a40868e8b0668685b359fe45bb7db86013eae4b2f93a9059abe3b1e`).
No Hugo build, release lookup or installer generation is required.

## Hosting

Serve the repository root as a static website. For GitHub Pages, select
**Deploy from a branch**, branch **main**, directory **/(root)**.
The custom domain is **devrig.dev**, recorded in `CNAME`.
`.nojekyll` preserves the prebuilt site files without Jekyll processing.
The pages use the original root-relative paths and devrig.dev URLs.

`install.sh`, `install.ps1`, `version.json`, `updatePlugins.xml`, the EULA,
documentation, release pages, CSS and SVG assets are included. Installer links
continue to point to the original GitHub release assets and pinned JDK vendors.

## Local preview

```sh
python3 -m http.server --directory . 8000
```

Open http://localhost:8000/. Paths resolve as they do at the domain root.
