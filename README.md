# Georgia Pre-Approval Eligibility Engine 🏠

[![Platform](https://img.shields.io/badge/Platform-GitHub_Pages-blue.svg)](https://pages.github.com/)
[![Built With](https://img.shields.io/badge/Built_With-HTML5%20%2F%20CSS3%20%2F%20JS-orange.svg)](#)
[![Deployment Status](https://img.shields.io/badge/Deployment-Live-success.svg)](#)

An interactive, high-converting client qualification engine built for **Marcus Albright (Senior Loan Officer, NMLS #1503465)**. This system replaces standard passive landing pages with an active dynamic utility tool optimized for converting cold traffic from Facebook Ads ("sofa scrollers") and Google Search.

---

## 🎯 Strategic Purpose

Traditional mortgage intake forms create massive friction, leading to abandoned carts and wasted ad spend. This platform captures high-intent leads by providing **instant consumer value first**—reverse-calculating a buyer's maximum housing budget and purchasing power range before guiding them seamlessly into the official secure Loan Factory application pipeline.

---

## ✨ Key Technical Architecture

* **Dynamic Employment Logic Branching:** If a user selects **"Self-Employed / 1099"**, the system dynamically alters the terminology and data labels to ask for *"Net Monthly Revenue (Bank Statement Averages)"* instead of standard corporate *"Gross Monthly Income"*, reducing friction for non-traditional borrowers.
* **2026 Loan Limit Validation:** Automatically benchmarks calculations against the updated Federal baseline conforming limit of **$832,750**. If estimated lending requirements cross this boundary, it instantly shifts flags from *Conforming* to *Jumbo Loan Category Required*.
* **Automated Data Query Hand-off:** Automatically records client contact entries (Name, Email) and financial profiles inside the browser session, compiling them seamlessly into outbound query strings to prevent secondary entry fields.

---

## 🛠️ Customization & Link Setup

To direct successful wizard applicants straight into your specific **Loan Factory portal dashboard**, update line **349** inside your `index.html` file:

```javascript
// Locate this block near the bottom of index.html and update the URL string:
const baseAppUrl = "[https://yourportal.loanfactory.com/apply](https://yourportal.loanfactory.com/apply)";
