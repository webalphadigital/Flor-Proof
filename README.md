# Flor Proof

**Every bouquet with its story.** Growers register each flower harvest and get a QR code. Customers scan it and see who grew the flowers, where they come from, which variety they are and how long they last. No app and no wallet needed.

- Live demo: https://webalphadigital.github.io/Flor-Proof/
- Guide for judges (how to test): https://webalphadigital.github.io/Flor-Proof/judges.html
- Backend repository: https://github.com/webalphadigital/flor-proof-backend

## The problem

Small and medium flower growers keep track of their harvests without a reliable method. Whoever buys a bouquet doesn't know who grew it, and without a brand growers can't build a reputation or keep customers coming back.

## How it works

1. **The grower registers a batch** (variety, zone, season, packages, harvest date, shelf life) and gets a QR code.
2. **The florist confirms receipt** of the batch and makes bouquets, each with its own QR code.
3. **The customer scans the QR** and sees the full journey, from grower to bouquet.

Each step is recorded on Monad Testnet through a smart contract, so the history of a batch can't be quietly edited afterwards. Growers and florists never handle a wallet: the backend signs for them.

## Pages

| File | Who uses it | What it does |
|---|---|---|
| `index.html` | Everyone | Home page: problem, solution, benefits and access to the forms |
| `productora.html` | Grower | Registers a batch and opens its QR |
| `florista.html` | Florist | Confirms receipt of a batch and makes a bouquet with its QR |
| `consulta.html` | Customer | Public lookup of a batch or bouquet, read straight from the contract |
| `qr.html` | Grower, florist | Shows a QR code and saves it as an image |
| `judges.html` | Judges | Testing guide, technical overview and links |

All pages are available in English and Spanish (EN | ES button).

## Run it

Plain HTML, CSS and JavaScript. There is no build step.

1. Publish the folder with GitHub Pages, or open the files in a browser.
2. In `consulta.html`, set the contract address in the `CONTRATO` constant.
3. In `productora.html` and `florista.html`, the `API` constant points to the backend.

## Smart contract

- Deployed on Monad Testnet.

## Built during the Monad Metropolis hackathon

The smart contract, the backend, the grower and florist forms, the public lookup page, the QR pages and the bilingual interface.

## Contact

fabianfigueroac@gmail.com

## License

Copyright 2026 Alpha Digital. All rights reserved. The code is public so it can be reviewed; it may not be copied, modified or redistributed without written permission.
