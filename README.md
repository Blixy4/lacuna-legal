# Lacuna legal pages

Static pages shown inside the app (webview) and linked from the Play Console.

- `privacy.html`: politique de confidentialité
- `terms.html`: conditions d'utilisation
- `delete-account.html`: how to delete the account and the data
- `index.html`, `style.css`, `fonts/` (Fraunces and Manrope, self-hosted, SIL Open Font License, no outside requests)

## Publish on GitHub Pages

1. Create a public repository named `lacuna-legal` under the account Blixy4.
2. Put the files of this folder at the root of the repository (not inside a subfolder).
3. Settings, Pages, Source: Deploy from a branch, branch `main`, folder `/ (root)`.
4. After a minute the pages are at `https://blixy4.github.io/lacuna-legal/privacy.html` and so on.

If the account or repository name is different, change `host` and `base` in
`lib/util/legal_links.dart`.

## Play Console

- App content, Privacy policy: `https://blixy4.github.io/lacuna-legal/privacy.html`
- App content, Data safety, account deletion link: `https://blixy4.github.io/lacuna-legal/delete-account.html`

## Keep in sync

The texts also exist inside the app (`LegalContent` in `lib/screens/legal_screen.dart`),
shown when the page cannot load. Both are generated from one source, so when a text
changes, change both and update the date.
