# Portal Knowledge Demo

Interactive prototype v1.0 for Portal document management and Smart help. Switch between Partner view and Admin view with the top controls.

## Run locally

```sh
python3 -m http.server 4182 --bind 127.0.0.1
```

Open http://127.0.0.1:4182/ from this folder. A web server is required; opening index.html directly will not load the mock directories. No build or package installation is required.

## Included flows

- Document upload (multiple files), required language, language/status filters, processing, publication, version replacement and original-file download.
- Assistant settings with account/country union availability and searchable multi-selects.
- Admin question testing and question records.
- Draggable Smart help entry on the partner dashboard.
- Relevant-file language priority: question language, Portal account language, then English.

## Prototype boundaries

All accounts, documents and answers are sample data. No production services, WeKnora, live AI or Portal APIs are connected. Browser storage keeps local edits and uploaded files; uploads are not sent to a server. Preseeded documents have no original file binary. Question-record CSV export is a product requirement and is not implemented in this prototype. Language detection is a limited local heuristic, and language options are illustrative.

This repository contains the runnable static demo only. It excludes credentials, source-audit snapshots, node_modules and other workspace projects.
