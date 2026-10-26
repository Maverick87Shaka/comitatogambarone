# Comitato Gambarone San Bovio — landing page

Pagina singola (`index.html`, no build, no dipendenze) raggiunta dagli striscioni tramite QR code.

- Contenuto: logo + nome comitato, location, slogan anti-ecomostro, CTA Facebook, CTA mailto per iscrizione.
- Email comitato: comitatogambarone@yahoo.com
- Pagina FB: https://www.facebook.com/profile.php?id=61591755391217
- Logo: `assets/logo.png` (fornito dal comitato, PNG con trasparenza, 357x350, rosso dominante #ff4700).

## Deploy

GitHub Pages (branch `main`, root della repo). Nessuna workflow: basta servire la root.
Anteprima locale: `python3 -m http.server 8099`.

## Repo

- `Maverick87Shaka/comitatogambarone` (pubblica, branch `main`).
- URL pubblico atteso: https://maverick87shaka.github.io/comitatogambarone/
  (da abilitare in Settings -> Pages: Deploy from a branch, `main` / `(root)`).
- Logo fornito dal comitato: PNG 357x350 con trasparenza (no fondo bianco).

## Note

- Mobile-first: pensata per la scansione QR in verticale, target di tap >= 60px, dark mode automatica.
- Il token GitHub usato in questo workspace non puo creare repo ne gestire Pages (serve PAT con scopes `repo` + `admin:repo`/Pages).
