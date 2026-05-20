# 🧘‍♀️ Serenity – Onboarding Email Template

[![Built With - MJML](https://img.shields.io/badge/Built%20With-MJML-22b573?style=flat-square)](https://mjml.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

LİVE PREVİEW: https://edayavuz6.github.io/Serenity-Saas-Email-Template/

A production-ready, bulletproof welcome and feature onboarding email template designed for **Serenity**, a fictional SaaS meditation platform. 

This project demonstrates professional email engineering workflows, showcasing semantic component structure, responsive visual hierarchy, and absolute cross-client email compatibility (including legacy Outlook clients).

---

## 🚀 Key Features

* **Complete New-User Flow:** Cohesive onboarding structure containing a hero moment, dual feature reveal, quick-start checklist, and conversion-focused primary CTA.
* **Dual Design Accent:** High-contrast layout using premium warm neutral tones (`#faf7f4`, `#f5f0eb`) paired with deep forest green (`#3d6b5e`) to deliver an editorial, trust-building aesthetic.
* **Typography Hierarchy:** Clean pairing of *DM Serif Display* (for elegant headers) and *DM Sans* (for modern body readability).

---

## 🛠️ Technical Decisions & Optimizations

| Area | Engineering Decision & Optimization |
| :--- | :--- |
| **Why MJML?** | Chosen over raw HTML to maintain a dry, component-based, version-controlled source file that automatically compiles into bulletproof table-based HTML, vendor-prefixed media queries, and Outlook VML. |
| **Preheader Teaser** | Injected a hidden, zero-height `<mj-text>` block at the very top to ensure custom, hand-crafted preview snippets in the user's inbox. |
| **Cross-Client Fonts** | External Google Fonts loaded with fallback serif stacks to guarantee graceful degradation if a client blocks network resources. |
| **Outlook-Safe CTA** | Built with semantic native `<mj-button>` elements ensuring clickable, filled VML buttons in Outlook instead of broken flat links. |
| **Performance** | The compiled production-ready HTML output is **~50 KB**, safely below the **102 KB Gmail clipping threshold**. |
| **Compliance** | Includes physical address hooks, unsubscription logic, and preference links ensuring CAN-SPAM and GDPR baselines. |

---

## 📂 Project Structure

```bash
├── index.mjml       # Source code (Clean, component-based editable file)
└── index.html       # Production build (Compiled, inlined, cross-client HTML)
