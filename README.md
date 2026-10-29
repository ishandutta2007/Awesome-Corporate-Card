# Awesome-Corporate-Card

## Top Corporate Card Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Business Charge Cards, Spend Controls & Self-Hosted Expense Infrastructure*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Corporate Cards**. These tools enable businesses to issue employee cards, set spending limits, automate receipt matching, and streamline expense reporting—turning company spend into a controlled, visible, and accountable operation.



**Examples** include Shopify Credit, Brex, Ramp, Mercury Card, Stripe Corporate Card, American Express Business, Capital On Tap, Rho Card, Torpago, and Divvy (BILL Spend & Expense) (the category leaders).



**Open-source emphasis**: Corporate Card is a domain where open-source tooling is **fundamentally limited by the card-issuing layer**. The strongest open-source projects are **Expensify's New Expensify** (MIT, 5,000+ stars, actively maintained, with corporate card management and receipt scanning)  and **FinPilot** (a full-stack expense approval system with multi-level workflows and receipt OCR) . **Stripe's sample apps** (issuing-treasury, platform-issuing) demonstrate how to *build* a corporate card program using Stripe Issuing—but they are reference implementations, not deployable products. **No open-source project replicates the integrated card-issuing, credit underwriting, and rewards engine** of Brex, Ramp, or Shopify Credit. The card itself (the Visa/Mastercard plastic) requires a banking partner and regulatory licensing that software alone cannot provide.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Shopify Credit](https://www.shopify.com/credit)**  

  Pay-in-full Visa® business card from Shopify, powered by Stripe and issued by Celtic Bank; **no credit checks or personal guarantee**; offers up to **3% cashback** on top spend category (marketing, fulfillment, or wholesale) and 1% on the rest; payment options include 1-month grace period or up to 10 months paid from daily sales for a fee . Virtual card on approval, physical card in 5-7 days.



- **[Brex](https://www.brex.com/)**  

  Corporate card and spend management platform with AI-powered controls, automated receipts, and expense assistant; Spring 2026 release adds **automatic ERP vendor creation** (NetSuite, Sage Intacct, QuickBooks Online, Xero), **foreign VAT reclaim** integration via Fintua and VAT IT, and Microsoft Dynamics 365 Business Central connectivity . Claims 71% of expenses handled entirely by automations.



- **[Ramp](https://ramp.com/)**  

  Corporate card and finance automation platform with **AI that proactively identifies savings**—flagging duplicate subscriptions, negotiating SaaS contracts, and alerting to unusual spending . Q1 2026 adds **real-time budget vs. actuals tracking**, **Accounting Agents** that code transactions with 98% accuracy and sync to ERP, and **Ramp Global** expansion to UK/EU with local payment rails (SEPA, BACS) and local issuing in Mexico and Brazil .



- **[Mercury Card (IO)](https://mercury.com/credit)**  

  Corporate card with **1.5% cashback on all spend**, no annual or interest fees; limits scale with cash balances held in Mercury; **no personal guarantee**; automatic reporting to major credit bureaus; built-in expense management with AI categorization and receipt matching . Available without a Mercury deposit account (IO-only) with linked external bank account for underwriting .



- **[Stripe Corporate Card](https://stripe.com/)**  

  Card issuing via **Stripe Issuing** (programmatic virtual/physical cards with real-time authorization and spend controls) and **Treasury** (prepaid debit cards drawing from a financial account, up to 100 cards per account, no coding required) . Requires a Stripe account and is designed for platforms building card programs rather than direct-to-business card offerings.



- **[American Express Business](https://www.americanexpress.com/)**  

  Suite of business credit cards including Business Platinum ($895 annual fee, travel/lounge perks), Delta SkyMiles Gold Business, Marriott Bonvoy Business, and Amazon Business Prime; rewards range from 1-6 points per dollar; most require personal guarantee and good credit .



- **[Capital On Tap](https://www.capitalontap.com/)**  

  UK business credit card with **1 point per £1** (redeemable for cash, gift cards, Avios, Virgin Points, or Radisson Rewards); no annual, foreign exchange, or ATM fees; unlimited employee cards with individual spending limits; **preloading feature** earns 1% cashback on preloaded spend (1.25% for Pro) . Requires personal guarantee; APR as low as 13.86% variable.



- **[Rho Card](https://www.rho.co/)**  

  Corporate card and spend management platform with **Expenses API** (read-only view of corporate card expenses with approval state, policy compliance, tags, and receipt attachments) . API-first design for integration into custom finance stacks.



- **[Torpago](https://pitchbook.com/profiles/company/432495-64)**  

  Corporate card and expense management platform designed for **banks to deliver credit experiences** to their business customers; provides virtual cards with expense automation . Founded 2019, raised ~$100M; positioned as infrastructure for bank-issued corporate cards rather than direct-to-business.



- **[Divvy (BILL Spend & Expense)](https://www.bill.com/product/corporate-cards)**  

  Corporate charge card with **no annual fees**, credit lines from $1,000 to $5M, and **performance-based rewards** (up to 7x points on restaurants, 5x on hotels with weekly payoff) . Enforceable budgets that stop overspending before it happens; unlimited virtual cards; deep ERP syncs (QuickBooks, NetSuite); reports to SBFE for business credit building . No interest charges (charge card, balance due in full).



## Open-Source GitHub Projects



### Expense Management Platforms



- **[Expensify (New Expensify)](https://github.com/Expensify/App)**  

  The largest open-source **expense management platform** available (MIT, 5,000+ GitHub stars, actively maintained with commits within hours) . Features corporate card management, **SmartScan receipt OCR** that extracts and categorizes data, automated approval workflows, real-time syncing across devices, global reimbursements in 160+ currencies, and integrations with accounting/HR/travel systems . **The most complete open-source expense platform**—but the card issuing and banking layer remains proprietary (Expensify's commercial card program).



- **[FinPilot](https://github.com/Abhinavhaldiya/FinPilot)**  

  Open-source enterprise **expense approval system** (React/Node.js/PostgreSQL) . Features smart claim submission with receipt uploads and auto-categorization, multi-currency support with real-time exchange rates, **receipt OCR**, multi-level approval workflows based on amount thresholds, role-based access (Employee, Manager, HR, Finance), budget tracking for departmental limits, audit trail, and PDF/Excel/CSV export . **Strong for reimbursement workflows and policy enforcement**—but lacks corporate card integration and real-time transaction feeds.



- **[Zemio](https://github.com/zemio-co/zemio)**  

  Open-source, self-hostable expense claim management platform for student initiatives (MIT, public beta) . Features expense reports with itemized expenses and receipt attachments (up to 5 files), **review workflow** (Draft → Pending Approval → Needs Revision/Accepted/Rejected → Paid), multi-tenant organizations, Microsoft OAuth, **encrypted banking details** snapshotted at submission, cost unit allocation, PDF export, and audit trail . **Best for small organizations** needing structured reimbursement workflows.



### Card Issuing Infrastructure (Build Your Own)



- **[Stripe Issuing + Treasury Sample Apps](https://github.com/stripe-samples/issuing-treasury)**  

  Official Stripe sample applications (Node.js) for building **corporate card programs** with Stripe Issuing and Treasury . Includes `expense-management` (commercial pre-funded card Issuing program) and `embedded-finance` (full-stack financial services) demos. Demonstrates virtual card creation, **MCC-based spending controls**, real-time authorization webhooks (2-second approval), and transaction monitoring. **Reference implementations**—not production-ready products, but the clearest open-source blueprint for building a card program.



- **[Platform Issuing Demo](https://github.com/kater-stripe/platform-issuing)**  

  Comprehensive demo of **Stripe Connect + Issuing** for building payment platforms with virtual card issuance . Features account onboarding, balance management, virtual cards, **MCC-based restrictions** (allowed: restaurants/transportation/cosmetics; blocked: gas stations/gambling), spending limits (£25/day, £500/month), and **real-time webhook-based transaction approval** (2-second decisions) . **The most detailed open-source reference** for implementing spend controls on issued cards.



### Additional Strong Open-Source Options



- **Cajachica** — Open-source expense approval system (Node.js/PostgreSQL) with multi-level approvals, receipt OCR, and audit trails; similar scope to FinPilot but less active .

- **No open-source corporate card issuer exists** — The card plastic, credit underwriting, banking partnerships, and regulatory compliance (KYC/AML, capital requirements) that underpin Brex, Ramp, or Shopify Credit are not replicable by open-source software. Stripe's samples show how to *integrate* with an issuing provider, not how to *become* one.



**Frameworks for building custom systems**: For **expense management and reimbursement workflows**, Expensify (if using their platform) or FinPilot/Zemio (if self-hosting) provide functional foundations . For **building a card program**, Stripe Issuing samples demonstrate the integration pattern—but require a Stripe account, banking partner, and compliance infrastructure . No open-source project provides the integrated card + spend controls + rewards + underwriting stack of Ramp or Brex.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Corporate card platforms handling payment card data must comply with **PCI DSS** requirements; card issuing requires banking partnerships, KYC/AML compliance, and regulatory licensing that open-source software cannot provide.

- **Open-source corporate cards are limited to the expense management layer**—Expensify, FinPilot, and Zemio provide expense workflows, and Stripe samples demonstrate card program integration . However, **no open-source project replicates the integrated card issuing, credit underwriting, and rewards engine** of Brex, Ramp, or Shopify Credit. Businesses seeking a corporate card should evaluate commercial providers; those building a card program should use Stripe Issuing or similar BaaS with proper compliance infrastructure.

- Verify license terms for commercial use; Expensify uses MIT , FinPilot is open-source , Zemio uses MIT , and Stripe samples are provided under Stripe's terms.



---



**Made for finance teams, spend managers, and fintech builders exploring corporate card infrastructure.**  

Let's make corporate spend management more open at the software layer, but with clear eyes about the banking and underwriting infrastructure that software cannot replace.
