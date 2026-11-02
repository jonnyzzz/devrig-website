# devrig.dev website

This repository hosts the prebuilt website originally developed in
[jonnyzzz/mcp-steroid](https://github.com/jonnyzzz/mcp-steroid), including its
[`website/` Hugo sources](https://github.com/jonnyzzz/mcp-steroid/tree/680b7985686f3f0011708cc2f2c704ebcf755e94/website)
and generated installer and update files. It was populated from a downloaded
snapshot of the live **https://devrig.dev/** website on **2 November 2026**.

## Origin and import

| Item | Source |
|---|---|
| Original project | [MCP Steroid / devrig](https://github.com/jonnyzzz/mcp-steroid) |
| Upstream website deployment commit | [`680b7985686f3f0011708cc2f2c704ebcf755e94`](https://github.com/jonnyzzz/mcp-steroid/commit/680b7985686f3f0011708cc2f2c704ebcf755e94) |
| Upstream deployment | [GitHub Pages run 31218444119](https://github.com/jonnyzzz/mcp-steroid/actions/runs/31218444119), completed 7 August 2026 |
| Downloaded website | https://devrig.dev/, captured 2 November 2026 |
| Published product version | **0.102** ([upstream release v0.102](https://github.com/jonnyzzz/mcp-steroid/releases/tag/v0.102)) |
| Import archive | `devrig.dev-published-0.102-2026-11-02.tar.gz` |
| Archive SHA-256 | `0141d8c07a40868e8b0668685b359fe45bb7db86013eae4b2f93a9059abe3b1e` |

All **42 website content files** were copied unchanged from that archive. They
include the HTML pages, documentation, release notes, CSS, SVG assets, EULA,
`install.sh`, `install.ps1`, `version.json` and `updatePlugins.xml`.
The archive was made from the deployed HTTP responses; it was not rebuilt from
the source commit or recovered from the original CI build artifact.

The separate hosting setup consists of `CNAME`, `.nojekyll` and this repository's
documentation. The `devrig.dev` GitHub Pages domain binding was moved from
`jonnyzzz/mcp-steroid` to this repository on 2 November 2026.
No Hugo build, release lookup or installer generation is needed to publish these files.

## Attribution and licensing

The upstream project distributes its source under the **Apache License, Version 2.0**.
[LICENSE](LICENSE) contains an informational provenance note followed by a verbatim
copy of the [upstream license at the deployment commit](https://github.com/jonnyzzz/mcp-steroid/blob/680b7985686f3f0011708cc2f2c704ebcf755e94/LICENSE),
including its original copyright notices:

- Copyright 2025-2026 Eugene Petrenko (mcp@jonnyzzz.com)
- Copyright 2025-2026 JetBrains

Existing notices in the imported website files are preserved. This repository
retains those upstream attributions and license terms.

The included [EULA](EULA) is a separate upstream document for the **compiled MCP
Steroid plugin binaries**. The website's installer and download links still point
to the original GitHub release assets and pinned JDK vendors; those external
binaries and services retain their own applicable terms.

## Hosting

Serve the repository root as a static website. GitHub Pages is configured for
**Deploy from a branch**, branch **main**, directory **/(root)**.
The custom domain is **devrig.dev**, recorded in `CNAME`.
`.nojekyll` preserves the prebuilt site files without Jekyll processing.
The pages use the original root-relative paths and devrig.dev URLs.

## Local preview

```sh
python3 -m http.server --directory . 8000
```

Open http://localhost:8000/. Paths resolve as they do at the domain root.
