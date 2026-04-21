# 🏭 Procure-to-Pay (P2P) System — TechEdge Manufacturing

A full-stack **SAP MM Procure-to-Pay simulation model** built as a web application demonstrating the complete purchasing cycle from Purchase Requisition to Vendor Payment.

---

## 📋 Project Overview

| Detail | Value |
|--------|-------|
| **Project Type** | SAP MM P2P Process Simulation |
| **Company** | TechEdge Manufacturing Pvt. Ltd. (Fictitious) |
| **Company Code** | TE01 |
| **SAP Module** | MM (Materials Management) + FI Integration |
| **Institute** | KIIT University |

---

## 🚀 Live Demo

Open `index.html` directly in any browser — **no server or installation required**.

---

## 📦 P2P Process Flow Implemented

```
ME51N → ME54N → ME21N → MIGO → MIRO → F-53
  PR   Approve   PO    GR    Invoice  Payment
```

| Step | T-Code | Description |
|------|--------|-------------|
| 1 | ME51N | Create Purchase Requisition |
| 2 | ME54N | PR Approval (Release Strategy) |
| 3 | ME21N | Create Purchase Order from PR |
| 4 | MIGO  | Goods Receipt (Movement Type 101) |
| 5 | MIRO  | Logistics Invoice Verification |
| 6 | F-53  | Vendor Payment Processing |

---

## ✨ Features

- **Dashboard** with real-time KPIs (Open PRs, POs, GR count, Pending Invoices)
- **P2P Flow Diagram** with live step highlighting
- **Purchase Requisition** creation and approval workflow (ME51N / ME54N)
- **Purchase Order** creation with vendor assignment (ME21N)
- **Goods Receipt** posting with stock update (MIGO)
- **3-Way Matching** — PO ↔ GR ↔ Invoice with variance detection (MIRO)
- **Payment Processing** with accounting document simulation (F-53)
- **Audit Trail** with complete document chain and GR/IR accounting entries
- Fully interactive — create, approve, and track documents end-to-end

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Styling | Custom CSS (no frameworks — zero dependencies) |
| Data | In-memory JavaScript state |
| Deployment | Static file (open index.html) |

---

## 📁 Project Structure

```
p2p_model/
├── index.html      ← Complete P2P application (single file)
└── README.md       ← This file
```

---

## 🎓 SAP Concepts Demonstrated

- **Organisational Structure**: Company Code → Plant → Storage Location → Purchasing Org
- **Master Data**: Vendor Master, Material Master, Purchase Info Record
- **3-Way Match**: Purchase Order ↔ Goods Receipt ↔ Vendor Invoice
- **GR/IR Clearing**: Automatic accounting entries on GR and MIRO posting
- **Release Strategy**: PR approval workflow before PO creation
- **Document Flow**: PR → PO → Material Doc → Accounting Doc → Invoice → Payment

---

## 🚀 How to Run

1. Download or clone this repository
2. Open `index.html` in any browser
3. Navigate through the P2P modules using the left sidebar

No npm, no build step, no server — just open and run.

---

## 📄 License

MIT — Free to use for educational purposes.
