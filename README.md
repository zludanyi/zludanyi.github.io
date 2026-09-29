# Domain association

This repository publishes verification files for `https://zludanyi.github.io/`.

## GitHub Pages

In Settings > Pages, choose **Deploy from a branch**, branch **main**, folder **/(root)**. The `.nojekyll` file enables publishing the `.well-known` directory as static files.

## Android passkeys

The association endpoint is `https://zludanyi.github.io/.well-known/assetlinks.json`. It must return HTTP 200 with an `application/json` content type and no redirect.

The initial association is an empty JSON array. It authorizes no Android app until the SHA-256 certificate fingerprint from the actual signed APK is available and the matching credential-sharing statement is added. An empty file is deployment preparation, not a working passkey association.

The certificate fingerprint is public verification metadata. Keep private signing keys and passwords out of this repository.
