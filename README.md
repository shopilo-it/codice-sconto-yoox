# Codice sconto YOOX, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto YOOX** da [shopilo.it](https://shopilo.it/negozi/yoox.com). Restituisce **coupon YOOX** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-yoox](https://shopilo-it.github.io/codice-sconto-yoox/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-yoox
cd codice-sconto-yoox
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "YOOX",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su moda e design di lusso",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/yoox.com"
  }
]
```

## Coupon YOOX disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su moda e design di lusso | [shopilo.it](https://shopilo.it/negozi/yoox.com) |

Codici attivi: **[shopilo.it/negozi/yoox.com](https://shopilo.it/negozi/yoox.com)**

## Domande frequenti

### Come utilizzo un codice sconto YOOX?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/yoox.com), aggiungi i prodotti al carrello su YOOX e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon YOOX?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher YOOX piu recenti?
La pagina [shopilo.it/negozi/yoox.com](https://shopilo.it/negozi/yoox.com) viene aggiornata quotidianamente con i codici sconto YOOX, voucher YOOX e coupon promozionali YOOX piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su YOOX

YOOX e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/yoox.com) trovi i migliori codici sconto YOOX, coupon YOOX verificati e voucher YOOX attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-yoox
```

```javascript
const { fetchCoupons } = require('codice-sconto-yoox');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
