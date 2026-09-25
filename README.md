# qbo-callback

Public pages for Adam Isaacson's private QuickBooks Online reader ("Books Reader"), served by
GitHub Pages at https://adam-isaacson.github.io/qbo-callback/.

- `index.html` - home and launch URL
- `privacy.html`, `terms.html` - the privacy policy and licence Intuit requires for production keys
- `disconnected.html` - the disconnect landing page
- `callback/` - the production redirect URI. Intuit only redirects to https, never localhost,
  so this page forwards `code`, `state` and `realmId` to the local helper on
  `http://127.0.0.1:8790/callback`, which holds the client secret and does the token exchange.

No secrets live here, and no page collects data.
