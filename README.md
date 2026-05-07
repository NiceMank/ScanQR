# ScanQR

Page web “blague” faite pour être ouverte via un QR code.

## Contenu

- Grand titre : **Yakooooo**
- Message : **Tu peux pas acheter forfait ? C'est décevant**
- Image principale (locale) : `sticker-enfant-bebe-leopard-removebg-preview.png`
- Décoration animée : plusieurs petites images `rire.png` qui bougent en arrière-plan

## Fichiers importants

- `index.html`
- `rire.png`
- `sticker-enfant-bebe-leopard-removebg-preview.png`

Important : sous Linux, le nom de fichier est sensible à la casse. Le fichier attendu est `rire.png` (minuscule).

## Lancer en local

Option 1 : ouvrir directement `index.html` dans le navigateur.

Option 2 (recommandé) : servir le dossier avec un mini serveur HTTP.

Avec Python :

```bash
python3 -m http.server 8080
```

Puis ouvre :

```text
http://localhost:8080/
```

## Utiliser avec un QR code

- Mets ce dossier sur un hébergement (ou ton serveur local accessible sur le réseau).
- Génère un QR code qui pointe vers l’URL de la page (ex: `http://IP_DE_TON_PC:8080/`).

## Personnalisation rapide

- Texte : modifie le `<p>` et la `<div class="hint">` dans `index.html`.
- Nombre d’images animées : duplique/supprime des `<img src="./rire.png" ...>` dans la `<div class="decor">`.