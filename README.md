# Codice sconto Lentiamo, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Lentiamo** da [shopilo.it](https://shopilo.it/negozi/lentiamo.it). Restituisce **coupon Lentiamo** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-lentiamo](https://shopilo-it.github.io/codice-sconto-lentiamo/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-lentiamo
cd codice-sconto-lentiamo
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Lentiamo",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su lenti a contatto",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/lentiamo.it"
  }
]
```

## Coupon Lentiamo disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su lenti a contatto | [shopilo.it](https://shopilo.it/negozi/lentiamo.it) |

Codici attivi: **[shopilo.it/negozi/lentiamo.it](https://shopilo.it/negozi/lentiamo.it)**

## Domande frequenti

### Come utilizzo un codice sconto Lentiamo?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/lentiamo.it), aggiungi i prodotti al carrello su Lentiamo e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Lentiamo?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Lentiamo piu recenti?
La pagina [shopilo.it/negozi/lentiamo.it](https://shopilo.it/negozi/lentiamo.it) viene aggiornata quotidianamente con i codici sconto Lentiamo, voucher Lentiamo e coupon promozionali Lentiamo piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Lentiamo

Lentiamo e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/lentiamo.it) trovi i migliori codici sconto Lentiamo, coupon Lentiamo verificati e voucher Lentiamo attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-lentiamo
```

```javascript
const { fetchCoupons } = require('codice-sconto-lentiamo');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
