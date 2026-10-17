# Damm-Apps – F-Droid-Repo

Eigenes F-Droid-Repo für **DammBoard**, **DammZeit**, **DammLauncher** und **DammZahlen**. Ein Workflow holt alle zwei
Stunden die neuesten GitHub-Releases, baut den signierten Index mit `fdroidserver` und
veröffentlicht ihn über GitHub Pages.

**Repo-Adresse für F-Droid:**
`https://teyro.github.io/damm-fdroid/repo?fingerprint=db7f158b6eb2c7eb17e79aa4a9ae0e9487c3c2228fe7de60b37a1979408c0604`

Anleitung mit QR-Code: https://teyro.github.io/damm-fdroid/

- Die APKs werden nicht neu gebaut, sondern unverändert aus den Releases übernommen.
- Neue App ins Repo: Namen in `APPS` (Workflow) eintragen und `metadata/<paketname>.yml` anlegen.
- Sofort neu bauen: Actions → F-Droid-Repo → *Run workflow* (mit „erzwingen“).
- Secrets: `FDROID_KEYSTORE_BASE64`, `FDROID_KEYSTORE_PASS` (Repo-Schlüssel, Sicherung liegt offline).
