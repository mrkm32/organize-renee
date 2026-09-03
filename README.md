# Renee Family Care & Financial Organization Hub

A secure, client-side encrypted web application and reimbursement management system for **Mark & Shelly Matthews**, **Laurie Salse**, and **Autumn Aguilar** to organize **Renee Termine's** past-due bills, preserve her estate assets, coordinate her transition to safe memory care, and ensure full legal reimbursement from the pending reverse mortgage.

---

## 🔒 Security & Privacy (Zero-Knowledge Architecture)

This repository contains **NO sensitive financial plaintext, account numbers, addresses, or VINs**.
- All family financial data, account numbers, debt balances, and vehicle records are stored inside a client-side **AES-256 GCM encrypted vault** derived using **PBKDF2 (100,000 iterations)**.
- Without the master family passphrase, the repository data is completely unreadable ciphertext.
- All local spreadsheet exports (`renee_financial_ledger.csv`) are excluded via `.gitignore` and remain strictly on local authorized devices.

---

## 👥 Family Coordination Team & Roles

| Family Member | Designated Role | Primary Responsibilities |
| :--- | :--- | :--- |
| **Autumn Aguilar** | **Legal Power of Attorney & Authorized Representative (Attorney-in-Fact)** | Legally in charge. Sole authorized signatory for vehicle title transfers (DMV Form REG 227) and reverse mortgage closing disclosures. Formally approves family reimbursement claims. |
| **Laurie Salse** | **On-Site Care Coordinator & Primary Family Liaison** | On-scene staying with Renee in Sun City. Assesses day-to-day cognitive and physical safety, organizes physical mail/bills, and **escorts Renee in person to Chase Bank** to open a clean checking account and report fraud. Eligible for reverse mortgage reimbursement for on-scene advances. |
| **Mark & Shelly Matthews** | **Financial Sponsors & Operational Administrators** | Advancing immediate capital to cure utility arrears and stop storage lien foreclosure. Managing debt settlement negotiations, maintaining the centralized encrypted ledger, and preparing reverse mortgage audit documentation. |

---

## 🌟 Accessing the Hub on GitHub Pages

1. Navigate to: **`https://mrkm32.github.io/organize-renee/`**
2. **Unlock**: Enter your private family passphrase.
3. Once entered, the browser's native Web Crypto API decrypts the confidential bills, vintage vehicle records, and reimbursement claims directly into your browser session.
4. When you finish, click **"Lock Vault"** or close the browser tab.

---

## ⚖️ Reverse Mortgage Reimbursement & Settlement

- **Editable Ledger**: Out-of-pocket reimbursement claims can be edited at any time to adjust amounts, payees, payment methods, reference numbers, or notes.
- **Receipt Evidence Attachments (Photos & PDFs)**: Attach photos (JPEG, PNG, HEIC) or scanned PDF receipts to any ledger entry. Photos are automatically compressed client-side to preserve razor-sharp legibility while keeping storage minimal.
- **Interactive Receipt Viewer**: Click any receipt badge to view documents full-screen, rotate camera photos 90° clockwise, preview embedded PDFs, or download files.
- **Server-Side GitHub Cloud Sync**: End-to-end encrypted synchronization via GitHub API (`vault.json`). Allows seamless multi-device syncing across iPhones, iPads, and PCs while keeping all data client-side encrypted.
- **IndexedDB High-Capacity Storage**: Browser storage upgraded to IndexedDB, providing gigabytes of capacity for receipts and documents without running into traditional 5MB `localStorage` limits.
- **Payer Tracking**: Every payment can be attributed to **Mark & Shelly Matthews**, **Laurie Salse**, or **Autumn Aguilar**.
- **Formal Settlement Statement**: Clicking **"Print Formal Settlement Statement"** generates an audit-ready legal accounting statement with receipt proof statuses for the reverse mortgage escrow officer or attorney.
- **Three Signature Blocks**:
  1. **Autumn Aguilar** (Attorney-in-Fact / Power of Attorney for Renee Termine)
  2. **Laurie Salse** (Claimant / On-Site Care Coordinator)
  3. **Mark & Shelly Matthews** (Claimants / Financial Sponsors)

---

## 🤝 Debt Negotiation & Settlement Tracking

Before paying overdue balances, the system supports negotiating discounts:
- Track settlement offers, discounts, and fee waivers.
- Automatic calculation of estate savings when a settlement is agreed.
- Payment modal automatically pre-fills with negotiated discount amounts.

---

## 🚐 California DMV Planned Non-Operation (PNO) Strategy

- **Save ~$790 with Planned Non-Operation (PNO)**: Filing PNO online at [dmv.ca.gov](https://www.dmv.ca.gov/portal/vehicle-registration/vehicle-registration-renewal/planned-non-operation-pno/) costs **~$25/vehicle** instead of paying full registration ($150–$220+ each) for stored vintage vans.
- **Selling the Vehicles**: Autumn Aguilar (as POA) signs title transfer forms (REG 227 / REG 262) to sell vintage collectible vehicles, generating cash for Renee's care and eliminating monthly storage fees.
