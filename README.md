# Limepay (limepay)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
