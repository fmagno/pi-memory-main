---
description: >-
  Ongoing analysis matching Aemarco Contabilidade invoices with bank payments
  from Francisco Magno Morgado Lda (Novobanco statements)
updated: '2026-03-11'
tags:
  - aemarco
  - accounting
  - invoices
  - novobanco
  - reconciliation
  - francisco-morgado
---
# Aemarco Contabilidade — Invoice Reconciliation

## Context
- **Company:** Francisco Magno Morgado Lda
- **Bank:** Novobanco Empresas
- **Account:** IBAN PT50 0007 0000 0080 2202 4172 3
- **Source files:** `/Users/francisco.morgado/Downloads/novobanco_docs_20260311010116/` (folders 001–010, each with a PDF bank statement)
- **Extracted invoices:** `/tmp/aemarco_invoices/` (extracted from notmuch emails)

## Bank Statements Analysed
| Folder | Statement | Period |
|--------|-----------|--------|
| 001 | Extrato 1/2026 | Dec 2025 – Jan 2026 |
| 002 | Extrato 2/2026 | Jan 2026 – Feb 2026 |
| 003 | Extrato 3/2025 | Apr 2025 – May 2025 |
| 004 | Extrato 4/2025 | May 2025 – Jun 2025 |
| 005 | Extrato 5/2025 | Jun 2025 – Jul 2025 |
| 006 | Extrato 6/2025 | Jul 2025 – Aug 2025 |
| 007 | Extrato 7/2025 | Aug 2025 – Sep 2025 |
| 008 | Extrato 8/2025 | Sep 2025 – Oct 2025 |
| 009 | Extrato 9/2025 | Oct 2025 – Nov 2025 |
| 010 | Extrato 10/2025 | Nov 2025 – Dec 2025 |

## Full Invoice–Payment Reconciliation

| Invoice | Date | Period | Line Items | Total | Bank Payment Date | Bank Ref | Status |
|---------|------|--------|------------|-------|-------------------|----------|--------|
| FT 2025A3/443 | 2025-04-10 | Abril 2025 | Contabilidade €125 + Admin €6 + Livros Selados €34.96 | **€204.13** | 19.07.2025 | Trf Cred Sepa+ Online 588031643 | ✅ Matched |
| FT 2025A3/646 | 2025-05-30 | Maio 2025 | Contabilidade €125 | **€153.75** | 19.07.2025 | Trf Cred Sepa+ Online 588031406 | ✅ Matched |
| FT 2025A3/727 | 2025-06-17 | Maio 2025 (Admin) | Serviços Administrativos €6 | **€7.38** | 19.07.2025 | Trf Cred Sepa+ Online 588031321 | ✅ Matched |
| FT 2025A3/785 | ~2025-06-27 | Julho 2025 | Contabilidade €125 (est.) | **€153.75** | 19.07.2025? | — | ⚠️ In CC, no invoice PDF |
| FT 2025A3/1012 | 2025-08-19 | Agosto 2025 | Contabilidade + Admin | **€161.13** | 22.08.2025 | Trf Cred Sepa+ Online 594807743 | ✅ Matched |
| FT 2025A3/1150 | 2025-09-18 | Setembro 2025 | Contabilidade + Admin | **€161.13** | 18.09.2025 | Trf Cred Sepa+ Online 600573961 | ✅ Matched |
| FT 2025A3/1287 | 2025-10-16 | Outubro 2025 | Contabilidade + Admin | **€161.13** | 20.10.2025 | Trf Cred Sepa+ Online 607327255 | ✅ Matched |
| FT 2025A3/1429 | 2025-11-17 | Novembro 2025 | Contabilidade + Admin | **€161.13** | 20.11.2025 | Trf Cred Sepa+ Online 614150204 | ✅ Matched |
| FT 2025A3/1595 | 2025-12-18 | Dezembro 2025 | Contabilidade + Admin | **€161.13** | 20.12.2025 | Trf Cred Sepa+ Online 621144773 | ✅ Matched |
| FT 2026A3/1723 | 2026-01-16 | Janeiro 2026 | Contabilidade €130 + Admin €6 | **€167.28** | 19.01.2026 | Trf Cred Sepa+ Online 627497450 | ✅ Matched |
| FT 2026A3/1874 | 2026-02-18 | Fevereiro 2026 | Contabilidade €130 + Admin €6 | **€167.28** | 25.02.2026 | Trf Cred Sepa+ Online 635248759 | ✅ Matched |

**Note:** Also in Extrato 3/2025 there is a payment on 08.05.25 of €153.75 (Trf Cred Sepa+ Nbnet 573239244) — this likely corresponds to **FT 2025A3/354** (Mar 2025 invoice, due 27.04.2025), paid slightly late in May.

## Key Clarifications

### €204.13 on 19.07.25 (Bank payment #4)
**Confirmed as Factura 443 (Abril 2025):** this was the first Aemarco invoice after company incorporation, and included an extra line:
- Contabilidade Organizada: €125.00 (VAT 23%)
- Serviços Administrativos: €6.00 (VAT 23%)
- **Livros Selados (Stamped books):** €34.96 (VAT 23%) — one-time setup cost
- Total IVA: €38.17 → **TOTAL: €204.13**
- NOT a food subsidy. ✅

### €7.38 on 19.07.25 (Bank payment #2)
**Confirmed as Factura 727 (Maio 2025 — Serviços Administrativos only):** €6.00 + 23% VAT = **€7.38**. Invoiced separately from the main accounting fee (Factura 646).

### July 2025 — Three payments on same day (19.07.25)
All three were catch-up payments for invoices 443 (Apr), 646 (May), 727 (May admin), and very likely also **785** (Jul). The Conta Corrente shows Recibos 671/672/673 all on 24.07.2025 settling invoices 443, 646, 727. Bank payments preceded by a few days.

### Price evolution
| Period | Monthly Fee (before VAT) | Total (incl. VAT) |
|--------|--------------------------|-------------------|
| Apr–Jul 2025 | €125 contab + €6 admin | €153.75 (normal months) |
| Aug–Dec 2025 | Higher base (price increase) | **€161.13** |
| Jan 2026+ | €130 contab + €6 admin | **€167.28** |

## Missing / Outstanding

| Invoice | Period | Status |
|---------|--------|--------|
| FT 2025A3/354 | Mar 2025 | Paid 08.05.25 (Extrato 3) but no invoice PDF available |
| FT 2025A3/785 | Jul 2025 | In Conta Corrente — no invoice PDF retrieved yet |
| FT 2026A3/1874 | Feb 2026 | **UNPAID** — due 20 Mar 2026 — €167.28 to IBAN PT50 0036 0487 9910 6002 0088 5 |

## Email Sources

| Invoice | Email thread / File |
|---------|---------------------|
| 443, 646, 727 | notmuch thread:00000000000005f9 (Guia para pagamento) |
| 1012 | notmuch thread:00000000000005f9 |
| 1150, 1287, 1429 | notmuch thread:00000000000005f9 |
| 1595 | notmuch thread:00000000000005f9 (Factura nº 1595.pdf) |
| 1723, 1874 | notmuch thread:0000000000005420 (FATURAS, Fri 06 Mar 2026) |
| Conta Corrente | notmuch thread:00000000000016b6 (CONTA CORRENTE, Oct 2025) |

## Next Actions

- [ ] **Pay FT 2026A3/1874 (Fevereiro 2026)** — €167.28 to IBAN PT50 0036 0487 9910 6002 0088 5 — due 20 Mar 2026
- [ ] **Pay FT 2026A3/1723 (Janeiro 2026)** — €167.28 — **OVERDUE** (was due 15 Feb 2026) — same IBAN
- [ ] Retrieve invoice PDF for FT 2025A3/785 (Jul 2025) if needed for accounting records
- [ ] Confirm with Odete/Ana Nogueira that the reconciliation matches their records
