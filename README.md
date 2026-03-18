[README.md](https://github.com/user-attachments/files/26086257/README.md)
# M&A Tax Due Diligence — Process Map

An interactive process map for the **M&A Tax Due Diligence** workflow at Henkel, built as a single-page web application.

## 🔗 Live Site

👉 **[https://lucaprocoder.github.io/m-a-tax-DD/](https://lucaprocoder.github.io/m-a-tax-DD/)**

---

## 📋 Overview

This tool provides an interactive overview of the full M&A Tax Due Diligence process — from deal initiation through to closing and integration. It is designed for internal use by the Henkel Tax Function and M&A team.

The process is structured into **5 phases** with **15 steps** in total:

| Phase | Name | Steps |
|-------|------|-------|
| 00 | Pre-DD / Deal Initiation | Pre-Information, RFP to Advisors, Kick-Off Meeting |
| 01 | Data Room & Analysis | Data Room Opening, Q&A Process, Expert Call |
| 02 | Interim Reporting | Flash Update 1 & 2, Preliminary DD Executive Summary |
| 03 | Final DD & Contracts | Draft Contracts Review, Final DD Report, InvestCom / MBM |
| 04 | Signing & Closing | Final Bid, Signing of Contracts, Closing & Integration |

---

## 🖱️ How to Use

1. **Select a phase** by clicking on one of the tabs at the top
2. **Click on a step** in the left panel to open detailed information
3. The right panel shows the **title, description and key items** for each step

---

## 🛠️ How to Update Content

All content is stored in the `phases` variable inside the `<script>` section at the bottom of `index.html`. Each step follows this structure:

```js
{
  name: "Step Name",               // shown in the left panel
  title: "Full Step Title",        // shown in the detail panel header
  desc: "Description text...",     // shown as body text
  keys: [
    { label: "Key Item", sub: "Short description" },
    ...
  ],
  tags: ["Tag1", "Tag2"]           // shown as labels at the bottom
}
```

To update content, edit `index.html` directly in GitHub using the ✏️ edit button, then click **"Commit changes"**. The site updates automatically within 1–2 minutes.

---

## 📁 Repository Structure

```
m-a-tax-DD/
└── index.html      # Single-page application (all code + content)
└── README.md       # This file
```

---

## ⚠️ Note on Confidentiality

This repository is currently set to **Public**, meaning the site is accessible to anyone with the link. As long as only placeholder or general process content is used this is acceptable. Once confidential deal-specific information is added, consider switching to a **private hosting solution** (e.g. Henkel SharePoint / Intranet).

---

*Henkel AG & Co. KGaA · Tax Function · Internal Use Only*
