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

- Mobile-first: pensata per la scansione QR in verticale, dark mode automatica.
- Vincolo accettato dal committente: tutta la pagina deve stare in UNA schermata su telefoni piccoli
  (test di riferimento 360x570, OnePlus One). Compatto tramite breakpoint su max-ALTEZZA (700px, 560px),
  non sulla larghezza. Misurare con iframe + bottom dell'ultimo elemento, non con scrollHeight
  (gonfiato da min-height:100svh). Non ridurre i bottoni sotto ~50px: sono i tap target primari.
- QR da stampare generati in `qr/` (ignorato da git): livello correzione H, testato con zxing-cpp.
- Il token GitHub usato in questo workspace non puo creare repo ne gestire Pages (serve PAT con scopes `repo` + `admin:repo`/Pages).
