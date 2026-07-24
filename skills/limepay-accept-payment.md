---
name: limepay-accept-payment
description: Create an order and take a card or BNPL payment through the Limepay Payments API, then optionally capture a pre-authorised transaction or refund it.
api: limepay:limepay-payments-api
generated: '2026-07-24'
method: generated
source: >-
  Grounded in the real documented operationIds of the Limepay Payments API as
  recorded in apis.yml and llms/limepay-llms.txt. No OpenAPI is retrievable
  (developer portal gated), so request/response bodies are described from the
  documented operation semantics, not from a live schema — treat field names as
  indicative and confirm against the (gated) developer portal.
operations:
  - CreateOrder
  - PayOrder
  - CaptureTransaction
  - CancelUncapturedTransaction
  - GetTransactionByOrderId
  - CreateRefund
  - GetPayPlanEligibilityMaxAmount
---

# Accept a payment with Limepay

Take a card or buy-now-pay-later (BNPL) payment for a purchase.

> Historical note: Limepay was acquired by Spenda (2024) and continued as April
> Solutions. The `api.limepay.com.au` host is retired and the developer portal is
> gated. This skill documents the real, historically public flow.

## Auth

Use a **Bearer** API key. Frontend/Checkout calls use the **Publishable** key;
server-side calls (capture, refund) use the **Secret** key. Send it as
`Authorization: Bearer <api_key>`.

## Steps

1. **(Optional) Check BNPL eligibility.** Call `GetPayPlanEligibilityMaxAmount`
   to confirm the buyer can finance the order amount as instalments before
   presenting the pay-later option.
2. **Create the order.** Call `CreateOrder` with the purchase amount, currency
   (AUD) and line items. Keep the returned order id.
3. **Take payment.** Call `PayOrder` for the order, supplying the payment
   source (a card token from Checkout, a saved card, or a wallet payment such as
   Apple Pay / Google Pay). For card payments this runs 3-D Secure as required.
4. **(Pre-auth flows) Capture.** If the order was authorised but not captured,
   call `CaptureTransaction` to settle it, or `CancelUncapturedTransaction` to
   void the authorisation and release the hold.
5. **Look up the transaction.** Use `GetTransactionByOrderId` to fetch the
   authorisation/capture record for the order.
6. **(If needed) Refund.** Call `CreateRefund` against the paid order to reverse
   all or part of the amount.

## Conventions

- **Amounts** are in the smallest currency unit; currency is AUD.
- **Wallets & 3DS** are handled inside `PayOrder`; no separate step.
- **Errors**: confirm error-envelope shape in the developer portal — the
  machine-readable error catalog is not publicly retrievable.
