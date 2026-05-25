# Asaas (asaas)

Asaas is a Brazilian financial-services and payments platform headquartered in Joinville, SC. It operates as a Banco Central-authorized payment institution and simplified credit company (SCD), offering small and medium businesses a digital account ("Conta Asaas") combined with collection, billing, and receivables tooling. The Asaas API (v3) at api.asaas.com is a REST/JSON surface covering Customers, Charges (Cobranças), Subscriptions, Installments, Pix (including Pix Automático recurring), Boleto, Credit Card, Checkout sessions, Payment Links, Split Payments, Transfers, Bill Payments, Anticipation of Receivables, Subaccounts / White-label, Invoices (Nota Fiscal), Escrow, Chargeback handling, Webhooks, and supporting services like Serasa default reporting, cell-phone recharges, and SMS / WhatsApp / email notifications. A full sandbox at sandbox.asaas.com, an Atlassian-hosted status page, a Discord developer community, and an llms.txt-indexed documentation site round out the developer experience. Asaas does not publish a first-party SDK on a GitHub org; the ecosystem is served by third-party community SDKs in Node.js, PHP, Python, Go, and Ruby plus e-commerce plugins for WooCommerce, Magento, and Nuvemshop.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/asaas/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Payments, Billing, Subscriptions, Pix, Boleto, Credit Card, Checkout, Split Payments, Webhooks, Digital Account, Receivables, Invoicing, Brazil, Fintech, SMB

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Asaas Customers API
Create, retrieve, update, list, and delete customers ("clientes"). The Customer object holds personal/business identifiers (CPF/CNPJ), contact details, address, default notification preferences, and Serasa-reporting configuration; it is the parent entity for charges, subscriptions, and installments.

**Human URL:** [https://docs.asaas.com/reference/criar-novo-cliente](https://docs.asaas.com/reference/criar-novo-cliente)

#### Tags:

 - Customers, CRM, CPF, CNPJ

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-novo-cliente)

### Asaas Charges (Cobranças) API
Core billing endpoint for creating individual charges payable by Boleto, Pix, Credit Card, Debit Card, or "undefined" (let the payer choose). Supports capture, refund, partial refund, anticipation, fine and interest configuration, discount rules, due-date updates, and status retrieval.

**Human URL:** [https://docs.asaas.com/reference/criar-nova-cobranca](https://docs.asaas.com/reference/criar-nova-cobranca)

#### Tags:

 - Charges, Billing, Refunds, Boleto, Pix, Credit Card

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-nova-cobranca)

### Asaas Subscriptions API
Recurring-billing subscriptions with weekly, biweekly, monthly, bimonthly, quarterly, semiannual, and annual cycles. Supports end-date or open-ended schedules, automatic charge generation per cycle, value updates, billing-type changes, and pause / cancel.

**Human URL:** [https://docs.asaas.com/reference/criar-nova-assinatura](https://docs.asaas.com/reference/criar-nova-assinatura)

#### Tags:

 - Subscriptions, Recurring, Billing Cycles

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-nova-assinatura)

### Asaas Installments (Parcelamentos) API
Generate a fixed series of installment charges from a single installment plan - typical for splitting a total amount across N monthly boletos or credit-card charges.

**Human URL:** [https://docs.asaas.com/reference/criar-novo-parcelamento](https://docs.asaas.com/reference/criar-novo-parcelamento)

#### Tags:

 - Installments, Parcelamento, Billing

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-novo-parcelamento)

### Asaas Pix API
Endpoints for Pix instant payments - static and dynamic QR codes, Pix keys (CPF/CNPJ/email/phone/random), QR code decoding, transfer via Pix, and the new Pix Automático (recurring authorized Pix debits, publicly released January 2026).

**Human URL:** [https://docs.asaas.com/reference/criar-cobranca-via-pix](https://docs.asaas.com/reference/criar-cobranca-via-pix)

#### Tags:

 - Pix, QR Code, Instant Payments, Pix Automático, Recurring

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-cobranca-via-pix)

### Asaas Boleto API
Issue, retrieve, and reconcile Brazilian boleto bancário (bank slip) charges, with configurable fines, interest, discounts, and due-date updates. Includes a webhook event for cancellation of expired slips.

**Human URL:** [https://docs.asaas.com/reference/criar-nova-cobranca](https://docs.asaas.com/reference/criar-nova-cobranca)

#### Tags:

 - Boleto, Bank Slip, Brazil, Billing

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-nova-cobranca)

### Asaas Credit Card API
Tokenize credit cards client-side and process card charges server-side, including pre-authorization (capture later), capture, refund, and 3DS challenge handling. Supports recurring use of tokenized cards across subscriptions and installments.

**Human URL:** [https://docs.asaas.com/reference/criar-nova-cobranca](https://docs.asaas.com/reference/criar-nova-cobranca)

#### Tags:

 - Credit Card, Tokenization, 3DS, Pre Authorization

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-nova-cobranca)

### Asaas Checkout API
Hosted checkout sessions that bundle one or more products / charges into a shareable payment URL. Supports multiple billing types, tax-document collection, and post-payment redirection.

**Human URL:** [https://docs.asaas.com/reference/criar-checkout](https://docs.asaas.com/reference/criar-checkout)

#### Tags:

 - Checkout, Hosted, Sessions

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-checkout)

### Asaas Payment Links API
Generate reusable payment links ("links de pagamento") for one-off or recurring collection over WhatsApp, SMS, email, or social. Each link can carry a fixed or buyer-defined amount.

**Human URL:** [https://docs.asaas.com/reference/criar-link-de-pagamento](https://docs.asaas.com/reference/criar-link-de-pagamento)

#### Tags:

 - Payment Links, Collection, WhatsApp

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-link-de-pagamento)

### Asaas Split Payments API
Configure split rules on a charge so that the net amount is automatically distributed across one or more wallet IDs at settlement time - the basis for marketplaces and platforms built on Asaas.

**Human URL:** [https://docs.asaas.com/reference/split-de-pagamentos](https://docs.asaas.com/reference/split-de-pagamentos)

#### Tags:

 - Split, Marketplace, Settlement

#### Properties

- [Documentation](https://docs.asaas.com/reference/split-de-pagamentos)

### Asaas Transfers API
Move funds out of the Asaas digital account: TED to external banks, Pix transfers to keys or banking details, and internal transfers between Asaas accounts, with optional scheduling.

**Human URL:** [https://docs.asaas.com/reference/criar-transferencia](https://docs.asaas.com/reference/criar-transferencia)

#### Tags:

 - Transfers, TED, Pix, Banking

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-transferencia)

### Asaas Bill Payments API
Pay external bills (boletos, concessionárias, GPS, DARF) from the Asaas digital account, with barcode-line lookup and scheduled execution.

**Human URL:** [https://docs.asaas.com/reference/pagar-uma-conta](https://docs.asaas.com/reference/pagar-uma-conta)

#### Tags:

 - Bill Payments, Banking, Boleto, Tax

#### Properties

- [Documentation](https://docs.asaas.com/reference/pagar-uma-conta)

### Asaas Anticipations (Antecipação) API
Anticipate future receivables - boleto, card, and Pix - to receive funds before the original settlement date in exchange for a discount fee. Endpoints simulate, request, and list anticipations.

**Human URL:** [https://docs.asaas.com/reference/listar-antecipacoes](https://docs.asaas.com/reference/listar-antecipacoes)

#### Tags:

 - Anticipation, Receivables, Credit

#### Properties

- [Documentation](https://docs.asaas.com/reference/listar-antecipacoes)

### Asaas Subaccounts / White-Label API
Create and manage subaccounts under a master account for white-label and BaaS use cases. Supports KYC document submission, activation links, per-subaccount API keys, and consolidated reporting.

**Human URL:** [https://docs.asaas.com/reference/criar-subconta](https://docs.asaas.com/reference/criar-subconta)

#### Tags:

 - Subaccounts, White Label, BaaS, KYC

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-subconta)

### Asaas Invoices (Nota Fiscal) API
Schedule, issue, and retrieve Brazilian electronic invoices (NFS-e) automatically tied to a charge or subscription, including municipal configuration and tax retention setup.

**Human URL:** [https://docs.asaas.com/reference/agendar-uma-nota-fiscal](https://docs.asaas.com/reference/agendar-uma-nota-fiscal)

#### Tags:

 - Invoices, NFSe, Tax, Compliance

#### Properties

- [Documentation](https://docs.asaas.com/reference/agendar-uma-nota-fiscal)

### Asaas Escrow Accounts API
Hold funds in escrow ("contas de garantia") until a release condition is met, with API-driven release or refund. Common in marketplaces where buyer-protection windows are required.

**Human URL:** [https://docs.asaas.com/reference/criar-conta-de-caucao](https://docs.asaas.com/reference/criar-conta-de-caucao)

#### Tags:

 - Escrow, Caução, Marketplace

#### Properties

- [Documentation](https://docs.asaas.com/reference/criar-conta-de-caucao)

### Asaas Chargebacks API
Retrieve and dispute credit-card chargebacks, including evidence upload and status retrieval.

**Human URL:** [https://docs.asaas.com/reference/listar-chargebacks](https://docs.asaas.com/reference/listar-chargebacks)

#### Tags:

 - Chargebacks, Disputes, Card

#### Properties

- [Documentation](https://docs.asaas.com/reference/listar-chargebacks)

### Asaas Account Balance & Statement API
Retrieve the current account balance and the financial statement (extrato) of credits and debits for the Asaas digital account.

**Human URL:** [https://docs.asaas.com/reference/obter-saldo-atual-da-conta](https://docs.asaas.com/reference/obter-saldo-atual-da-conta)

#### Tags:

 - Balance, Statement, Extrato

#### Properties

- [Documentation](https://docs.asaas.com/reference/obter-saldo-atual-da-conta)

### Asaas Cell Phone Recharge API
Top up Brazilian prepaid mobile lines by carrier and amount, debiting the Asaas account balance.

**Human URL:** [https://docs.asaas.com/reference/realizar-uma-recarga-de-celular](https://docs.asaas.com/reference/realizar-uma-recarga-de-celular)

#### Tags:

 - Recharge, Mobile, Prepaid

#### Properties

- [Documentation](https://docs.asaas.com/reference/realizar-uma-recarga-de-celular)

### Asaas Webhooks API
Event-driven HTTP callbacks for payment, subscription, transfer, anticipation, chargeback, account, and invoice events. Webhooks require a token (auto-generated as of Feb 2026) and Asaas signs requests for receiver-side verification.

**Human URL:** [https://docs.asaas.com/reference/configurando-o-webhook](https://docs.asaas.com/reference/configurando-o-webhook)

#### Tags:

 - Webhooks, Events, Notifications

#### Properties

- [Documentation](https://docs.asaas.com/reference/configurando-o-webhook)

## Common Properties

- [Website](https://www.asaas.com/)
- [SignUp](https://www.asaas.com/cadastro)
- [Documentation](https://docs.asaas.com/)
- [APIReference](https://docs.asaas.com/reference)
- [GettingStarted](https://docs.asaas.com/docs/visao-geral)
- [Authentication](https://docs.asaas.com/docs/autenticacao-no-asaas)
- [Sandbox](https://sandbox.asaas.com/)
- [ChangeLog](https://docs.asaas.com/changelog)
- [BreakingChanges](https://docs.asaas.com/docs/breaking-changes)
- [StatusPage](https://status.asaas.com/)
- [Pricing](https://www.asaas.com/precos)
- [TermsOfService](https://www.asaas.com/termos-de-uso)
- [PrivacyPolicy](https://www.asaas.com/politica-de-privacidade)
- [Support](https://central.ajuda.asaas.com/hc/pt-br)
- [HelpCenter](https://central.ajuda.asaas.com/hc/pt-br)
- [Blog](https://blog.asaas.com/)
- [LLMsTxt](https://docs.asaas.com/llms.txt)
- [Discord](https://discord.gg/asaas)
- [LinkedIn](https://www.linkedin.com/company/asaas/)
- [Instagram](https://www.instagram.com/asaas/)
- [YouTube](https://www.youtube.com/@asaas)

## Features

| Name | Description |
|------|-------------|
| Digital Account | Free monthly Conta Asaas with Mastercard debit card and unlimited internal transfers, positioned as a banking layer for SMBs. |
| Pix Automático | Recurring authorized Pix debits for subscription-style billing in BRL, publicly released January 2026 alongside webhook support. |
| Split Payments | Native marketplace splitting that distributes settled funds across multiple wallet IDs per charge. |
| Anticipation of Receivables | On-demand or automatic anticipation of boleto, card, and Pix receivables against a discount fee. |
| White-Label Subaccounts | Create and KYC subaccounts via API for white-label and BaaS platforms; each subaccount has its own API key. |
| Automated Dunning | Built-in notification engine over SMS, email, WhatsApp, and voice bot to chase overdue invoices; Asaas advertises ~80% default reduction. |
| Escrow Accounts | Funds-in-guarantee accounts release on API-driven conditions for marketplace buyer protection. |
| NFS-e Issuance | Schedule and issue Brazilian municipal NFS-e tied to a charge or subscription with tax-retention configuration. |
| Serasa Reporting | Optional default reporting and credit-score lookups via Serasa tied to customer records. |
| Sandbox | Full-feature sandbox.asaas.com environment for end-to-end integration testing before production. |

## Use Cases

| Name | Description |
|------|-------------|
| Recurring SaaS Billing | Subscriptions API plus Pix Automático, boleto, or card to bill Brazilian SaaS customers in BRL with automated dunning. |
| Marketplace Settlement | Split Payments + Subaccounts + Escrow let marketplaces collect, hold, and disburse to sellers natively in BRL. |
| Service-Business Collections | Service businesses (clinics, schools, gyms) automate billing, NFS-e issuance, and overdue-payment chasing via the Asaas dunning engine. |
| White-Label / BaaS | ISVs embed Asaas under their brand using Subaccounts, KYC, and per-account API keys to ship a payments product without a banking stack. |
| E-commerce Checkout | Checkout sessions and payment links plug into custom storefronts and supported plugins for one-click Pix / boleto / card. |

## Integrations

| Name | Description |
|------|-------------|
| WooCommerce | Official Asaas plugin for WordPress / WooCommerce stores. |
| Magento | Asaas extension for Magento 2 storefronts. |
| Nuvemshop | Native Asaas integration for Nuvemshop / Tiendanube Brazilian merchants. |
| Pluga | No-code automation marketplace with Asaas triggers and actions for connecting to hundreds of SaaS tools. |
| Zapier | Community Zapier integrations bridge Asaas events to thousands of downstream apps. |

## Solutions

| Name | Description |
|------|-------------|
| Conta Asaas (Digital Account) | Free Brazilian digital account with debit card targeted at MEIs and SMBs. |
| Cobranças (Charges) | The core billing product covering boleto, Pix, and card via a single API and UI. |
| Whitelabel / BaaS | Subaccount-based product for partners building branded payments experiences on top of Asaas. |
| Asaas Pay | Checkout / payment-link product for accepting payments without a full integration. |

## Maintainers

**FN:** API Evangelist

**URL:** https://apievangelist.com
