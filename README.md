# Asaas

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Asaas is a Brazilian financial-services and payments platform headquartered in Joinville, SC. It operates as a Banco Central-authorized payment institution and simplified credit company (SCD), offering small and medium businesses a digital account ("Conta Asaas") combined with collection, billing, and receivables tooling. The Asaas API (v3) at api.asaas.com is a REST/JSON surface covering Customers, Charges (Cobranças), Subscriptions, Installments, Pix (including Pix Automático recurring), Boleto, Credit Card, Checkout sessions, Payment Links, Split Payments, Transfers, Bill Payments, Anticipation of Receivables, Subaccounts / White-label, Invoices (Nota Fiscal), Escrow, Chargeback handling, Webhooks, and supporting services like Serasa default reporting, cell-phone recharges, and SMS / WhatsApp / email notifications. A full sandbox at sandbox.asaas.com, an Atlassian-hosted status page, a Discord developer community, and an llms.txt-indexed documentation site round out the developer experience. Asaas does not publish a first-party SDK on a GitHub org; the ecosystem is served by third-party community SDKs in Node.js, PHP, Python, Go, and Ruby plus e-commerce plugins for WooCommerce, Magento, and Nuvemshop.

**Areas:** Payments · Billing · Subscription · Pix · Boleto · Credit Cards · Checkout · Split Payments · Webhook · Digital Account · Receivables · Invoicing

## Asaas on APIs.io

Everything profiled for Asaas is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/asaas/](https://apis.io/providers/asaas/)** — or go straight to one of the APIs or properties below.

### APIs (57)

- [Asaas Customers API](https://apis.io/apis/asaas/customers/) — Create, retrieve, update, list, and delete customers ("clientes"). The Customer object holds personal/business identifiers (CPF/CNPJ), contact details,…
- [Asaas Charges (Cobranças) API](https://apis.io/apis/asaas/charges/) — Core billing endpoint for creating individual charges payable by Boleto, Pix, Credit Card, Debit Card, or "undefined" (let the payer choose). Supports…
- [Asaas Subscriptions API](https://apis.io/apis/asaas/subscriptions/) — Recurring-billing subscriptions with weekly, biweekly, monthly, bimonthly, quarterly, semiannual, and annual cycles. Supports end-date or open-ended…
- [Asaas Installments (Parcelamentos) API](https://apis.io/apis/asaas/installments/) — Generate a fixed series of installment charges from a single installment plan - typical for splitting a total amount across N monthly boletos or credit-card…
- [Asaas Pix API](https://apis.io/apis/asaas/pix/) — Endpoints for Pix instant payments - static and dynamic QR codes, Pix keys (CPF/CNPJ/email/phone/random), QR code decoding, transfer via Pix, and the new…
- [Asaas Boleto API](https://apis.io/apis/asaas/boleto/) — Issue, retrieve, and reconcile Brazilian boleto bancário (bank slip) charges, with configurable fines, interest, discounts, and due-date updates. Includes a…
- [Asaas Credit Card API](https://apis.io/apis/asaas/credit-card/) — Tokenize credit cards client-side and process card charges server-side, including pre-authorization (capture later), capture, refund, and 3DS challenge…
- [Asaas Checkout API](https://apis.io/apis/asaas/checkout/) — Hosted checkout sessions that bundle one or more products / charges into a shareable payment URL. Supports multiple billing types, tax-document collection,…
- [Asaas Payment Links API](https://apis.io/apis/asaas/payment-links/) — Generate reusable payment links ("links de pagamento") for one-off or recurring collection over WhatsApp, SMS, email, or social. Each link can carry a fixed…
- [Asaas Split Payments API](https://apis.io/apis/asaas/split-payments/) — Configure split rules on a charge so that the net amount is automatically distributed across one or more wallet IDs at settlement time - the basis for…
- [Asaas Transfers API](https://apis.io/apis/asaas/transfers/) — Move funds out of the Asaas digital account: TED to external banks, Pix transfers to keys or banking details, and internal transfers between Asaas accounts,…
- [Asaas Bill Payments API](https://apis.io/apis/asaas/bill-payments/) — Pay external bills (boletos, concessionárias, GPS, DARF) from the Asaas digital account, with barcode-line lookup and scheduled execution.
- [Asaas Anticipations (Antecipação) API](https://apis.io/apis/asaas/anticipations/) — Anticipate future receivables - boleto, card, and Pix - to receive funds before the original settlement date in exchange for a discount fee. Endpoints…
- [Asaas Subaccounts / White-Label API](https://apis.io/apis/asaas/subaccounts/) — Create and manage subaccounts under a master account for white-label and BaaS use cases. Supports KYC document submission, activation links, per-subaccount…
- [Asaas Invoices (Nota Fiscal) API](https://apis.io/apis/asaas/invoices/) — Schedule, issue, and retrieve Brazilian electronic invoices (NFS-e) automatically tied to a charge or subscription, including municipal configuration and…
- [Asaas Escrow Accounts API](https://apis.io/apis/asaas/escrow/) — Hold funds in escrow ("contas de garantia") until a release condition is met, with API-driven release or refund. Common in marketplaces where…
- [Asaas Chargebacks API](https://apis.io/apis/asaas/chargebacks/) — Retrieve and dispute credit-card chargebacks, including evidence upload and status retrieval.
- [Asaas Account Balance & Statement API](https://apis.io/apis/asaas/account-balance/) — Retrieve the current account balance and the financial statement (extrato) of credits and debits for the Asaas digital account.
- [Asaas Cell Phone Recharge API](https://apis.io/apis/asaas/cell-phone-recharge/) — Top up Brazilian prepaid mobile lines by carrier and amount, debiting the Asaas account balance.
- [Asaas Webhooks API](https://apis.io/apis/asaas/webhooks/) — Event-driven HTTP callbacks for payment, subscription, transfer, anticipation, chargeback, account, and invoice events. Webhooks require a token…
- [Asaas Ações em sandbox API](https://apis.io/apis/asaas/asaas-a-es-em-sandbox-api/) — The Ações em sandbox API from Asaas — 3 operation(s) for ações em sandbox.
- [Asaas Antecipações API](https://apis.io/apis/asaas/asaas-antecipa-es-api/) — The Antecipações API from Asaas — 5 operation(s) for antecipações.
- [Asaas Anticipation API](https://apis.io/apis/asaas/asaas-anticipation-api/) — The Anticipation API from Asaas — 1 operation(s) for anticipation.
- [Asaas Assinaturas API](https://apis.io/apis/asaas/asaas-assinaturas-api/) — The Assinaturas API from Asaas — 8 operation(s) for assinaturas.
- [Asaas Cartão de crédito API](https://apis.io/apis/asaas/asaas-cart-o-de-cr-dito-api/) — The Cartão de crédito API from Asaas — 2 operation(s) for cartão de crédito.
- [Asaas Chargeback API](https://apis.io/apis/asaas/asaas-chargeback-api/) — The Chargeback API from Asaas — 3 operation(s) for chargeback.
- [Asaas Checkout API](https://apis.io/apis/asaas/asaas-checkout-api/) — The Checkout API from Asaas — 2 operation(s) for checkout.
- [Asaas Clientes API](https://apis.io/apis/asaas/asaas-clientes-api/) — The Clientes API from Asaas — 4 operation(s) for clientes.
- [Asaas Cobranças API](https://apis.io/apis/asaas/asaas-cobran-as-api/) — The Cobranças API from Asaas — 17 operation(s) for cobranças.
- [Asaas Cobranças com dados resumidos API](https://apis.io/apis/asaas/asaas-cobran-as-com-dados-resumidos-api/) — The Cobranças com dados resumidos API from Asaas — 8 operation(s) for cobranças com dados resumidos.
- [Asaas Configurações de Webhooks API](https://apis.io/apis/asaas/asaas-configura-es-de-webhooks-api/) — The Configurações de Webhooks API from Asaas — 3 operation(s) for configurações de webhooks.
- [Asaas Consulta Serasa API](https://apis.io/apis/asaas/asaas-consulta-serasa-api/) — The Consulta Serasa API from Asaas — 2 operation(s) for consulta serasa.
- [Asaas Conta Escrow API](https://apis.io/apis/asaas/asaas-conta-escrow-api/) — The Conta Escrow API from Asaas — 4 operation(s) for conta escrow.
- [Asaas Documentos de cobranças API](https://apis.io/apis/asaas/asaas-documentos-de-cobran-as-api/) — The Documentos de cobranças API from Asaas — 2 operation(s) for documentos de cobranças.
- [Asaas Envio de documentos White Label API](https://apis.io/apis/asaas/asaas-envio-de-documentos-white-label-api/) — The Envio de documentos White Label API from Asaas — 3 operation(s) for envio de documentos white label.
- [Asaas Estornos API](https://apis.io/apis/asaas/asaas-estornos-api/) — The Estornos API from Asaas — 2 operation(s) for estornos.
- [Asaas Extrato API](https://apis.io/apis/asaas/asaas-extrato-api/) — The Extrato API from Asaas — 1 operation(s) for extrato.
- [Asaas Informações e personalização da conta API](https://apis.io/apis/asaas/asaas-informa-es-e-personaliza-o-da-conta-api/) — The Informações e personalização da conta API from Asaas — 7 operation(s) for informações e personalização da conta.
- [Asaas Informações financeiras API](https://apis.io/apis/asaas/asaas-informa-es-financeiras-api/) — The Informações financeiras API from Asaas — 3 operation(s) for informações financeiras.
- [Asaas Informações fiscais API](https://apis.io/apis/asaas/asaas-informa-es-fiscais-api/) — The Informações fiscais API from Asaas — 9 operation(s) for informações fiscais.
- [Asaas Installment API](https://apis.io/apis/asaas/asaas-installment-api/) — The Installment API from Asaas — 2 operation(s) for installment.
- [Asaas Link de pagamentos API](https://apis.io/apis/asaas/asaas-link-de-pagamentos-api/) — The Link de pagamentos API from Asaas — 6 operation(s) for link de pagamentos.
- [Asaas Negativações API](https://apis.io/apis/asaas/asaas-negativa-es-api/) — The Negativações API from Asaas — 8 operation(s) for negativações.
- [Asaas Notas fiscais API](https://apis.io/apis/asaas/asaas-notas-fiscais-api/) — The Notas fiscais API from Asaas — 4 operation(s) for notas fiscais.
- [Asaas Notificações API](https://apis.io/apis/asaas/asaas-notifica-es-api/) — The Notificações API from Asaas — 2 operation(s) for notificações.
- [Asaas Pagamento de contas API](https://apis.io/apis/asaas/asaas-pagamento-de-contas-api/) — The Pagamento de contas API from Asaas — 4 operation(s) for pagamento de contas.
- [Asaas Parcelamentos API](https://apis.io/apis/asaas/asaas-parcelamentos-api/) — The Parcelamentos API from Asaas — 6 operation(s) for parcelamentos.
- [Asaas Pix API](https://apis.io/apis/asaas/asaas-pix-api/) — The Pix API from Asaas — 6 operation(s) for pix.
- [Asaas Pix Automático API](https://apis.io/apis/asaas/asaas-pix-autom-tico-api/) — The Pix Automático API from Asaas — 5 operation(s) for pix automático.
- [Asaas Pix Recorrente API](https://apis.io/apis/asaas/asaas-pix-recorrente-api/) — The Pix Recorrente API from Asaas — 5 operation(s) for pix recorrente.
- [Asaas Recargas de celular API](https://apis.io/apis/asaas/asaas-recargas-de-celular-api/) — The Recargas de celular API from Asaas — 4 operation(s) for recargas de celular.
- [Asaas Registro de Recebíveis API](https://apis.io/apis/asaas/asaas-registro-de-receb-veis-api/) — The Registro de Recebíveis API from Asaas — 1 operation(s) for registro de recebíveis.
- [Asaas Splits API](https://apis.io/apis/asaas/asaas-splits-api/) — The Splits API from Asaas — 4 operation(s) for splits.
- [Asaas Subcontas Asaas API](https://apis.io/apis/asaas/asaas-subcontas-asaas-api/) — The Subcontas Asaas API from Asaas — 5 operation(s) for subcontas asaas.
- [Asaas Transações Pix API](https://apis.io/apis/asaas/asaas-transa-es-pix-api/) — The Transações Pix API from Asaas — 5 operation(s) for transações pix.
- [Asaas Transfer API](https://apis.io/apis/asaas/asaas-transfer-api/) — The Transfer API from Asaas — 1 operation(s) for transfer.
- [Asaas Transferências API](https://apis.io/apis/asaas/asaas-transfer-ncias-api/) — The Transferências API from Asaas — 3 operation(s) for transferências.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Asaas Webhooks](https://apis.io/asyncapis/asaas/asaas-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Moved to /providers/asaas/](https://apis.io/servers/asaas/asaas/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Asaas Agentic Access](https://apis.io/agentic-access/asaas/asaas-agentic-access/)

#### JSON Schema (6)

The data models the API reads and writes.

- [PaymentGetResponseDTO](https://apis.io/schemas/asaas/asaas-payment-get-response-dto/)
- [PaymentLeanGetResponseDTO](https://apis.io/schemas/asaas/asaas-payment-lean-get-response-dto/)
- [PaymentLeanSaveWithCreditCardResponseDTO](https://apis.io/schemas/asaas/asaas-payment-lean-save-with-credit-card-response-dto/)
- [PaymentPixQrCodeResponseDTO](https://apis.io/schemas/asaas/asaas-payment-pix-qr-code-response-dto/)
- [WebhookConfigGetResponseDTO](https://apis.io/schemas/asaas/asaas-webhook-config-get-response-dto/)
- [WebhookConfigSaveRequestDTO](https://apis.io/schemas/asaas/asaas-webhook-config-save-request-dto/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Asaas Context](https://apis.io/jsonld/asaas/asaas-context/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Asaas API Rules](https://apis.io/rules/asaas/asaas-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Asaas Authentication](https://apis.io/security/asaas/asaas-authentication/)
- [Asaas Domain Security](https://apis.io/security/asaas/asaas-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.asaas.com/)
- [Documentation](https://docs.asaas.com/)
- [Getting started](https://docs.asaas.com/docs/visao-geral)
- [API reference](https://docs.asaas.com/reference)
- [Pricing](https://www.asaas.com/precos)
- [Support](https://central.ajuda.asaas.com/hc/pt-br)
- [Changelog](https://docs.asaas.com/changelog)
- [Blog](https://blog.asaas.com/)
- [Terms of service](https://www.asaas.com/termos-de-uso)
- [Privacy policy](https://www.asaas.com/politica-de-privacidade)
- [Status](https://status.asaas.com/)

## API Evangelist rating

**Kin Score 43.2** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 70.0 |
| Contract quality | 71.1 |
| Contract governance | 19.7 |
| Operational transparency | 42.1 |
| Developer ergonomics | 46.4 |
| Access clarity | 13.2 |

**Agent readiness 54.0** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 15.2** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/asaas/](https://apis.io/providers/asaas/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Asaas: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/asaas/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
