# Domain association

This repository publishes verification files for `https://zludanyi.github.io/`.

## GitHub Pages

In Settings > Pages, choose **Deploy from a branch**, branch **main**, folder **/(root)**. The `.nojekyll` file enables publishing the `.well-known` directory as static files.

## Android passkeys

The association endpoint is `https://zludanyi.github.io/.well-known/assetlinks.json`. It was verified on 29 September 2026 to return HTTP 200 with an `application/json` content type and no redirect.

The current credential-sharing statement authorizes Android package `com.zludany.renovision3d` with this SHA-256 signing-certificate fingerprint, obtained from the signature-verified APK:

```text
88:A8:16:EB:8A:7E:29:47:CC:A3:71:E7:4E:41:B5:09:E7:5A:55:36:CE:8F:90:2A:20:B1:39:8F:D6:B4:76:CD
```

The statement grants only `delegate_permission/common.get_login_creds`. Preserve existing statements when adding another app or signing certificate. A real-device passkey and PRF test is still needed to verify the complete authentication flow.

The certificate fingerprint is public verification metadata. Keep private signing keys and passwords out of this repository.
