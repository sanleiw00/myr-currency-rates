# MYR Currency Exchange Rates Viewer

A lightweight, single-file web application for viewing live exchange rates with Malaysian Ringgit (MYR) as the base currency.

**Live Demo:** [https://sanleiw00.github.io/myr-currency-rates/](https://sanleiw00.github.io/myr-currency-rates/)

## Quick Start

Open `index.html` in any modern web browser.

## Features

- **Live Exchange Rates** - Real-time rates from Frankfurter API (European Central Bank data)
- **Bidirectional Conversion** - View both MYR to Currency and Currency to MYR rates
- **Interactive Calculator** - Instant currency conversion with input fields
- **Pin Favorites** - Keep frequently used currencies at the top
- **Advanced Search** - Filter by currency code, country name, or currency name
- **Unlimited Access** - No rate limits or API restrictions

## Usage Guide

### Viewing Exchange Rates

All currencies are displayed automatically with current exchange rates upon loading.

### Converting Currencies

Enter amounts in the conversion columns:
- **Left column (MYR)** - Enter MYR amount to see equivalent in foreign currency
- **Right column (Currency)** - Enter foreign currency amount to see equivalent in MYR

Both columns update each other automatically in real-time.

### Pinning Currencies

Click the thumbtack icon next to any currency to pin it to the top of the list. Pinned currencies remain at the top and persist across browser sessions.

### Searching

Use the search bar to filter currencies by:
- Currency code (e.g., USD, EUR, JPY)
- Country or region (e.g., United States, Japan, Singapore)  
- Currency name (e.g., Dollar, Euro, Yen)

### Clearing Inputs

Click the "Clear All" button to reset all conversion inputs and clear the search filter.

## Technical Specifications

**Architecture:**
- Single HTML file with embedded CSS and JavaScript
- No external dependencies or build process required
- Pure vanilla JavaScript (ES6+)

**API:**
- Primary source: Frankfurter API
- Data provider: European Central Bank (ECB)
- Rate limits: None (unlimited requests)
- Fallback: ExchangeRate.host API

**Data:**
- Approximately 40 major world currencies
- Updates: Fresh data fetched on every page load
- Accuracy: Official ECB exchange rates

**Storage:**
- LocalStorage for pinned currency preferences
- Fallback cache for offline resilience

## Browser Requirements

- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- JavaScript enabled
- Internet connection for live rate updates
- LocalStorage enabled (for pin functionality)

## Supported Currencies

Major global currencies including:
USD, EUR, GBP, JPY, CNY, AUD, CAD, SGD, HKD, THB, INR, KRW, CHF, SEK, NOK, DKK, PLN, MXN, NZD, and more.

## Data Attribution

Exchange rate data provided by [Frankfurter API](https://www.frankfurter.app), based on official European Central Bank rates.

## License

Free to use for personal and commercial purposes.
