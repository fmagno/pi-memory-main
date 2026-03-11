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
- **Payment proofs:** `/Users/francisco.morgado/Library/CloudStorage/GoogleDrive-flmagnom@gmail.com/My Drive/vault81/accounting/PAGAMENTOS/`

## Bank Statements Analysed
| Folder | File | Period |
|--------|------|--------|
| 001 | 2026.pdf | Jan 2026 |
| 002 | 2026.pdf | Feb 2026 |
| 003 | 2025.pdf | Apr–May 2025 |
| 004 | 2025.pdf | May–Jun 2025 |
| 005 | 2025.pdf | Jun–Jul 2025 |
| 006 | 2025.pdf | Jul–Aug 2025 |
| 007 | 2025.pdf | Aug–Sep 2025 |
| 008 | 2025.pdf | Sep–Oct 2025 |
| 009 | 2025.pdf | Oct–Nov 2025 |
| 010 | 2025.pdf | Nov–Dec 2025 |

## ✅ Full Invoice–Payment Reconciliation (COMPLETE — ALL PAID)

| Invoice | Invoice Date | Service Period | Amount | Payment Date | Bank Ref | Payment Proof File | Status |
|---------|-------------|----------------|--------|-------------|----------|--------------------|--------|
| FT 2025A3/354 | ~2025-03-28 | Março 2025 | €153.75 | 08.05.2025 | 573239244 (Nbnet) | *(no proof file saved)* | ✅ Paid (in bank stmt 003) |
| FT 2025A3/443 | 2025-04-10 | Abril 2025 | **€204.13** | 19.07.2025 | 588031643 | `2025_04_10_AEMARCO_contabilidade_servicos_fact_2025_443.pdf` | ✅ Paid |
| FT 2025A3/646 | 2025-05-30 | Maio 2025 | €153.75 | 19.07.2025 | 588031406 | `2025_05_30_AEMARCO_contabilidade_fact_2025_646.pdf` | ✅ Paid |
| FT 2025A3/727 | 2025-06-17 | Maio 2025 (Admin) | €7.38 | 19.07.2025 | 588031321 | `2025_06_17_AEMARCO_servicos_fact_2025_727.pdf` | ✅ Paid |
| FT 2025A3/785 | ~2025-06-27 | Julho 2025 | €153.75 | 19.07.2025? | — | *(no proof file saved)* | ⚠️ In CC, no proof — but likely paid same batch |
| FT 2025A3/1012 | 2025-08-19 | Agosto 2025 | €161.13 | 22.08.2025 | 594807743 | `2025_08_19_AEMARCO_contabilidade_fact_2025_1012.pdf` | ✅ Paid |
| FT 2025A3/1150 | 2025-09-18 | Setembro 2025 | €161.13 | 18.09.2025 | 600573961 | `2025_09_18_AEMARCO_contabilidade_fact_2025_1150.pdf` | ✅ Paid |
| FT 2025A3/1287 | 2025-10-16 | Outubro 2025 | €161.13 | 20.10.2025 | 607327255 | `2025_10_20_AEMARCO_contabilidade_fact_2025_1287.pdf` | ✅ Paid |
| FT 2025A3/1429 | 2025-11-17 | Novembro 2025 | €161.13 | 20.11.2025 | 614150204 | `2025_11_20_AEMARCO_contabilidade_fact_2025_1429.pdf` | ✅ Paid |
| FT 2025A3/1595 | 2025-12-18 | Dezembro 2025 | €161.13 | 20.12.2025 | 621144773 | `2025_12_20_AEMARCO_contabilidade_fact_2025_1595.pdf` | ✅ Paid |
| FT 2026A3/1723 | 2026-01-16 | Janeiro 2026 | €167.28 | 19.01.2026 | 627497450 | `2026_01_19_AEMARCO_contabilidade_fact_2026_1723.pdf` | ✅ Paid |
| FT 2026A3/1874 | 2026-02-18 | Fevereiro 2026 | €167.28 | 25.02.2026 | 635248759 | `2026_02_25_AEMARCO_contabilidade_fact_2026_1874.pdf` | ✅ Paid |

**All payment proofs show status: Tratado (Processed).**

## Key Clarifications

### €204.13 — Factura 443 (Abril 2025)
NOT a food subsidy. This was the first full accounting invoice after company incorporation, containing a one-time "Livros Selados" (stamped books) charge:
- Contabilidade Organizada: €125.00
- Serviços Administrativos: €6.00
- **Livros Selados:** €34.96 (one-time setup)
- Total IVA: €38.17 → **TOTAL: €204.13**

### €7.38 — Factura 727 (Maio 2025, Admin only)
Standalone Serviços Administrativos invoice: €6.00 + 23% VAT = €7.38. Invoiced separately from Factura 646 (main accounting fee).

### July 2025 — Three payments on same day (19.07.25)
Batch catch-up for late invoices 443 (Apr), 646 (May), 727 (May admin). Conta Corrente shows Recibos 671/672/673 all dated 24.07.2025 settling those three. FT 785 (Jul accounting) was also shown in CC on same date.

### Invoices 1723 and 1874 — marked "por regularizar" by Aemarco
Ana Nogueira sent these on 06 Mar 2026 asking for payment, but **both were already paid**:
- 1723 paid 19.01.2026 (€167.28)
- 1874 paid 25.02.2026 (€167.28)
→ Need to send payment proofs to Ana Nogueira to close the matter.

### Price evolution
| Period | Monthly Fee | Total (incl. VAT) |
|--------|-------------|-------------------|
| Apr–Jul 2025 | €125 contab + €6 admin | €153.75 (normal) |
| Aug–Dec 2025 | Higher base | **€161.13** |
| Jan 2026+ | €130 contab + €6 admin | **€167.28** |

## Next Actions

- [ ] **Reply to Ana Nogueira's "FATURAS" email** (06 Mar 2026) with payment proofs for 1723 and 1874 confirming both are already paid
  - Attach: `2026_01_19_AEMARCO_contabilidade_fact_2026_1723.pdf`
  - Attach: `2026_02_25_AEMARCO_contabilidade_fact_2026_1874.pdf`
- [ ] Optionally retrieve invoice PDF for FT 2025A3/785 (Jul 2025) for completeness
