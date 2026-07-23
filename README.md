<div align="center">

# AXIOM DeFi Portfolio Dashboard

### A responsive, framework-free Web3 portfolio interface by **AXIOM VISUAL**

Track a simulated crypto portfolio, load current market snapshots from CoinGecko, explore responsive SVG performance charts, and interact with a demonstration token-swap experience.

[View Live Demo](https://axiom-ui-lab.github.io/deFi-dashboard/) · [Explore the Repository](https://github.com/axiom-ui-lab/deFi-dashboard)

</div>

---

## Overview

AXIOM DeFi Portfolio Dashboard is a frontend portfolio project that explores the visual and interaction patterns of a modern decentralized-finance interface.

The application combines a portfolio overview, asset-level market information, responsive chart controls, and a simulated exchange flow in a single-page dashboard built with native web technologies.

The project does not connect to a blockchain, execute real transactions, or connect to a production wallet.

---

## Features

### Portfolio Overview

- Calculates the total value of a demonstration crypto portfolio
- Displays a weighted 24-hour portfolio change
- Updates asset values from the latest available market snapshot
- Presents Bitcoin, Ethereum, Solana, and USD Coin holdings

### CoinGecko Market Data

- Requests current USD prices and 24-hour percentage changes
- Updates portfolio and token values after a successful response
- Uses built-in demonstration data when the external request is unavailable
- Requires no private API key

Market data is requested when the application starts. It is not continuously streamed or automatically refreshed on an interval.

### Portfolio Performance

- Responsive SVG line-and-area chart
- Selectable `1D`, `7D`, and `30D` ranges
- Re-renders when the viewport changes
- Caches generated data for each selected range

The performance chart uses locally generated demonstration data. It does not represent historical CoinGecko or blockchain records.

### Quick Swap

- Numeric amount validation
- Estimated token conversion values
- Reversible source and destination tokens
- Current rate calculation based on the loaded price snapshot
- Visual interaction feedback

The final swap action is a demonstration only and does not submit a transaction to a decentralized exchange.

### Wallet and Asset Interactions

- Demonstration wallet-connect control
- Interactive asset rows
- Demo feedback for token detail interactions

No real wallet provider, smart contract, or Web3 transaction library is connected.

---

## Technology

The project is built with:

- Semantic HTML5
- Responsive CSS
- Vanilla JavaScript
- CoinGecko Simple Price API
- Inline SVG
- GitHub Pages

There is no frontend framework, package manager, build process, or runtime dependency.

---

## Project Structure

```text
DeFi-Dashboard/
├── index.html
├── README.md
├── css/
│   └── style.css
└── js/
    └── main.js
```

---

## Run Locally

Clone the repository:

```bash
git clone https://github.com/axiom-ui-lab/DeFi-Dashboard.git
cd DeFi-Dashboard
```

Serve the project through a local HTTP server:

```bash
python -m http.server 8000
```

Open the application at:

```text
http://localhost:8000/
```

A local server is recommended because the application requests market data from an external API.

---

## Data and Demonstration Boundaries

| Area | Implementation |
|---|---|
| Asset prices | CoinGecko snapshot with local fallback data |
| 24-hour changes | CoinGecko snapshot with local fallback data |
| Portfolio holdings | Demonstration values stored in the frontend |
| Performance chart | Locally generated simulated data |
| Wallet connection | Demonstration interaction |
| Token swap | Demonstration calculation and confirmation |
| Blockchain transactions | Not implemented |

This distinction is intentional: the project demonstrates frontend product design and interaction architecture rather than production financial infrastructure.

---

## Responsive and Accessibility Considerations

The interface includes:

- Semantic page regions
- Explicit form labels and accessible names
- Keyboard-focusable controls
- Button states for selected chart ranges
- Mobile-friendly layout behavior
- Responsive chart rendering
- Reduced visual complexity on smaller screens

Accessibility and browser behavior should continue to be verified whenever interactions or layout rules are changed.

---

## Deployment

The public version is deployed through GitHub Pages:

```text
https://axiom-ui-lab.github.io/DeFi-Dashboard/
```

The repository is a static site and can be hosted without a server-side application.

---

## Design and Development

**Designed and built by AXIOM VISUAL**

GitHub: [axiom-ui-lab](https://github.com/axiom-ui-lab/)

This project is part of the AXIOM VISUAL frontend portfolio and focuses on responsive financial-interface design, data presentation, and framework-free interaction development.

---

## Project Status

The dashboard is a public portfolio demonstration.

It is suitable for exploring the interface and reviewing the frontend implementation. It is not a financial product, wallet service, trading platform, or source of investment advice.

---

## License

Copyright © AXIOM VISUAL.

All rights reserved unless a separate license is added to this repository.
