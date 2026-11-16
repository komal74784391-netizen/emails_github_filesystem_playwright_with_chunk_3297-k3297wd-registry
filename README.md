# Halden Systems - Capability Registry

Public catalog of the engineering tools and services Halden Systems offers to clients.
The published site is generated from the entries in `catalog/`.

## Entry format

Every entry is a Markdown file named after its slug. The YAML front matter
carries the page metadata:

| field | meaning |
| --- | --- |
| `title` | Display name |
| `route` | Path on the public site |
| `updated` | Last editorial update |
| `lifecycle` | `published` (live on the site) or `draft` (not yet published) |
| `home_url` | Marketing page |
| `docs_url` | Documentation |
| `source_url` | Public source checkout, when one exists (optional) |

## Release metadata

Implementation teams commit a `distribution.json` manifest to their repository.
Releases in the `stable` channel are signed builds cut from `main` and are
publicly installable. `preview` and `draft` entries are internal only and are
never offered publicly.

`repositories.json` lists the repositories that are registered as catalog
back-ends or as related internal projects.

<!-- registry-sync: 20261116T011214Z-2736 -->
