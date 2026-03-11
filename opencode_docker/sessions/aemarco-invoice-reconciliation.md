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

## Status: COMPLETE — Bean workspace-varu created

See bean `workspace-varu` and supporting sources at:
`.beans/workspace-varu/sources.md`

## Context
- **Company:** Francisco Magno Morgado Lda
- **Bank:** Novobanco Empresas — IBAN PT50 0007 0000 0080 2202 4172 3
- **Bank statements:** `/Users/francisco.morgado/Downloads/novobanco_docs_20260311010116/` (001–010)
- **Payment proofs:** `/Users/francisco.morgado/Library/CloudStorage/GoogleDrive-flmagnom@gmail.com/My Drive/vault81/accounting/PAGAMENTOS/`
- **Aemarco contact:** Ana Nogueira — ananogueira@aemarco.pt — 255 539 210
- **Payment IBAN (Montepio):** PT50 0036 0487 9910 6002 0088 5

## Month-by-Month Verdict

| Month | Invoice | Amount | Paid | Payment Date | Notes |
|-------|---------|--------|------|-------------|-------|
| Mar 2025 | FT354 | €153.75 | ✅ | 08.05.25 | Paid from personal Nbnet account |
| Apr 2025 | FT443 | €204.13 | ✅ | 19.07.25 | Incl. one-off Livros Selados €34.96 |
| Mai 2025 | FT646 + FT727 | €161.13 | ✅ | 19.07.25 | Batch catch-up |
| **Jun 2025** | **—** | **?** | **❌** | — | **No invoice ever sent or received** |
| **Jul 2025** | **FT785** | **€153.75** | **❌** | — | **In Aemarco CC but never emailed or paid** |
| Ago 2025 | FT1012 | €161.13 | ✅ | 22.08.25 | |
| Set 2025 | FT1150 | €161.13 | ✅ | 18.09.25 | |
| Out 2025 | FT1287 | €161.13 | ✅ | 20.10.25 | |
| Nov 2025 | FT1429 | €161.13 | ✅ | 20.11.25 | |
| Dez 2025 | FT1595 | €161.13 | ✅ | 20.12.25 | |
| Jan 2026 | FT1723 | €167.28 | ✅ | 19.01.26 | |
| Fev 2026 | FT1874 | €167.28 | ✅ | 25.02.26 | |

**Total paid = Total invoiced to you = €1,659.22 (zero difference)**

## Key Finding

Jun and Jul 2025 were **never invoiced to Francisco** despite Aemarco having internal CC entries (FT785 Jul, FT935 Jul, FT1134 Aug admin). These were never sent by email, never saved in PAGAMENTOS, and no payment proof exists. Francisco likely owes Aemarco ~€300–€315 for those two months.

## Next Actions (tracked in bean workspace-varu)
- [ ] Email Ana Nogueira requesting invoices for Jun and Jul 2025
- [ ] Pay invoices once received
- [ ] Save payment proofs to PAGAMENTOS folder
