# Codice sconto Amazon, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Amazon** da [shopilo.it](https://shopilo.it/negozi/amazon.it). Restituisce **coupon Amazon** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-amazon](https://shopilo-it.github.io/codice-sconto-amazon/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-amazon
cd codice-sconto-amazon
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Amazon",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su categorie selezionate",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/amazon.it"
  }
]
```

## Coupon Amazon disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su categorie selezionate | [shopilo.it](https://shopilo.it/negozi/amazon.it) |

Codici attivi: **[shopilo.it/negozi/amazon.it](https://shopilo.it/negozi/amazon.it)**

## Domande frequenti

### Come utilizzo un codice sconto Amazon?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/amazon.it), aggiungi i prodotti al carrello su Amazon e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Amazon?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Amazon piu recenti?
La pagina [shopilo.it/negozi/amazon.it](https://shopilo.it/negozi/amazon.it) viene aggiornata quotidianamente con i codici sconto Amazon, voucher Amazon e coupon promozionali Amazon piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Amazon

Amazon e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/amazon.it) trovi i migliori codici sconto Amazon, coupon Amazon verificati e voucher Amazon attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-amazon
```

```javascript
const { fetchCoupons } = require('codice-sconto-amazon');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
