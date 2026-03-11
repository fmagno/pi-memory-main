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

## Aemarco Contabilidade Payments Found

| # | Statement | Date | Bank Reference | Amount | Notes |
|---|-----------|------|----------------|--------|-------|
| 1 | Extrato 3/2025 | 08.05.25 | Trf Cred Sepa+ Nbnet 573239244 | €153,75 | ✅ Likely accounting fee |
| 2 | Extrato 5/2025 | 19.07.25 | Trf Cred Sepa+ Online 588031321 | €7,38 | ❓ Small adjustment? |
| 3 | Extrato 5/2025 | 19.07.25 | Trf Cred Sepa+ Online 588031406 | €153,75 | ✅ Likely accounting fee |
| 4 | Extrato 5/2025 | 19.07.25 | Trf Cred Sepa+ Online 588031643 | €204,13 | ❌ User suspects this is food subsidy, NOT accounting |
| 5 | Extrato 6/2025 | 22.08.25 | Trf Cred Sepa+ Online 594807743 | €161,13 | ✅ Accounting fee |
| 6 | Extrato 7/2025 | 18.09.25 | Trf Cred Sepa+ Online 600573961 | €161,13 | ✅ Accounting fee |
| 7 | Extrato 8/2025 | 20.10.25 | Trf Cred Sepa+ Online 607327255 | €161,13 | ✅ Accounting fee |
| 8 | Extrato 9/2025 | 20.11.25 | Trf Cred Sepa+ Online 614150204 | €161,13 | ✅ Accounting fee |
| 9 | Extrato 10/2025 | 20.12.25 | Trf Cred Sepa+ Online 621144773 | €161,13 | ✅ Accounting fee |
| 10 | Extrato 1/2026 | 19.01.26 | Trf Cred Sepa+ Online 627497450 | €167,28 | ✅ Accounting fee (price increase) |
| 11 | Extrato 2/2026 | 25.02.26 | Trf Cred Sepa+ Online 635248759 | €167,28 | ✅ Accounting fee |

## Key Observations
- Regular monthly fee was **€153,75** (May 2025), then increased to **€161,13** (Aug–Dec 2025), then to **€167,28** (Jan–Feb 2026)
- **€204,13** on 19.07.25 is disputed — user believes it may be a food subsidy payment, not an accounting fee (note: €204,00 appears elsewhere for Novo Banco food subsidy transfers)
- **€7,38** on 19.07.25 is unexplained — likely a small correction/adjustment
- July 2025 had 3 payments on the same day — possibly catching up on missed months (note: no Aemarco payment visible in Extrato 4/2025 Jun period)
- **Extrato 4/2025** (May–Jun 2025): NO Aemarco payment found in this period

## Next Step
- Search email inbox for messages from **@aemarco.pt**
- Match invoices to bank payments to confirm amounts and identify any missing payments
- Clarify the €204,13 and €7,38 transactions
- Thunderbird profiles found at: `~/Library/Thunderbird/Profiles/`
