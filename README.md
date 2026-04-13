# Code promo Sarenza, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Sarenza** depuis [shopilo.fr](https://shopilo.fr/reductions/sarenza.com). Renvoie les **coupons Sarenza** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-sarenza](https://shopilo-fr.github.io/code-promo-sarenza/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-sarenza
cd code-promo-sarenza
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Sarenza",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur les chaussures de marque",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/sarenza.com"
  }
]
```

## Coupons Sarenza disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur les chaussures de marque | [shopilo.fr](https://shopilo.fr/reductions/sarenza.com) |

Codes actifs : **[shopilo.fr/reductions/sarenza.com](https://shopilo.fr/reductions/sarenza.com)**

## Questions frequentes

### Comment utiliser un code promo Sarenza ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/sarenza.com), ajoutez les produits a votre panier sur Sarenza et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Sarenza ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Sarenza les plus recents ?
La page [shopilo.fr/reductions/sarenza.com](https://shopilo.fr/reductions/sarenza.com) est mise a jour quotidiennement avec les codes promo Sarenza, bons de reduction Sarenza et coupons promotionnels Sarenza les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Sarenza

Sarenza est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/sarenza.com), retrouvez les meilleurs codes promo Sarenza, coupons Sarenza verifies et bons de reduction Sarenza actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-sarenza
```

```javascript
const { fetchCoupons } = require('code-promo-sarenza');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
