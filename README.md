# Limepay (limepay)

Limepay was a Melbourne-based Australian embedded-payments and white-label buy-now-pay-later (BNPL) company that let merchants and platforms accept card payments and offer pay-in-instalments through a single drop-in checkout and a REST API. After a failed 2021 IPO, Limepay was acquired by ASX-listed Spenda in 2024 and its product line was continued under the **April Solutions** brand — the primary domain `limepay.com.au` now redirects to `meetapril.com`, and the `docs.limepay.com.au` developer portal is gated behind a Redocly login. This profile documents Limepay's real, historically public API family honestly; no machine-readable OpenAPI is currently downloadable.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/limepay/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/limepay/refs/heads/main/apis.yml)

## Tags

- Payments
- Australia
- BNPL
- Payment Gateway
- Checkout
- Embedded Payments
- White Label
- Card Payments
- Marketplace
- Instalments

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## APIs

### Limepay Payments API

REST API for accepting and managing card and BNPL payments — create and pay orders, capture or void authorised (pre-auth) transactions, issue refunds, save cards as payment sources, and run 3-D Secure and wallet payments (Apple Pay / Google Pay). Authenticated with Publishable (frontend) and Secret (server-side) API keys sent as Bearer tokens.

- **Human URL:** [https://docs.limepay.com.au/developer-portal/payments/](https://docs.limepay.com.au/developer-portal/payments/)

#### Properties

- [Documentation](https://docs.limepay.com.au/developer-portal/payments/)
- [API Reference](https://docs.limepay.com.au/developer-portal/api-reference)

### Limepay Platform API

REST API for platform and marketplace integrations to onboard and manage sub-merchants: create platform merchants, bank accounts and persons, run KYC/identification, retrieve merchant tokens and settlement reports, and issue platform refunds. Authenticated with a platform API key passed as a Bearer token.

- **Human URL:** [https://docs.limepay.com.au/developer-portal/platform/](https://docs.limepay.com.au/developer-portal/platform/)

#### Properties

- [Documentation](https://docs.limepay.com.au/developer-portal/platform/)
- [API Reference](https://docs.limepay.com.au/developer-portal/api-reference)

### Limepay Checkout

Embeddable, customisable checkout that merchants drop into a web store (plugins for WooCommerce, Magento, PrestaShop and Salesforce Commerce Cloud) to accept card payments and present the pay-in-instalments (BNPL) option.

- **Human URL:** [https://docs.limepay.com.au/developer-portal/checkout-integration/](https://docs.limepay.com.au/developer-portal/checkout-integration/)

#### Properties

- [Documentation](https://docs.limepay.com.au/developer-portal/checkout-integration/)

## Common Properties

- [Website](https://www.limepay.com.au/) (redirects to meetapril.com)
- [Developer Portal](https://docs.limepay.com.au/developer-portal/) (login-gated)
- [Documentation](https://docs.limepay.com.au/developer-portal/)
- [API Reference](https://docs.limepay.com.au/developer-portal/api-reference)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
