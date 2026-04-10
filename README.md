# Cod reducere Amazon — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere Amazon** de pe [shopilo.it](https://shopilo.it/magazin/amazon.it). Returneaza **cupoane Amazon** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-amazon](https://shopilo-it.github.io/codice-sconto-amazon/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-amazon
cd codice-sconto-amazon
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Amazon",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su categorie selezionate",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/amazon.it"
  }
]
```

## Cupoane Amazon disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% di sconto su categorie selezionate | [shopilo.it](https://shopilo.it/magazin/amazon.it) |

Codurile active: **[shopilo.it/magazin/amazon.it](https://shopilo.it/magazin/amazon.it)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Amazon?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/amazon.it), adauga produsele in cos pe Amazon, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Amazon?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Amazon?
Pagina [shopilo.it/magazin/amazon.it](https://shopilo.it/magazin/amazon.it) este actualizata zilnic cu cele mai noi cod reducere Amazon, voucher Amazon si cupon promotional Amazon.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Amazon

Amazon este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/amazon.it) cele mai bune cod reducere Amazon, cupoane Amazon verificate si voucher Amazon active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-amazon
```

```javascript
const { fetchCoupons } = require('codice-sconto-amazon');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)
