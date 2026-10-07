# Invoice Manager – Invoice & Billing App

A simple, fast invoice generator and billing tracker that runs entirely in the browser. No backend, no sign-up, no build step. Create professional A4 invoices, track payments, and print or download them as PDF.

## Features

- **Dashboard**: total revenue, total / paid / pending invoices, and recent invoices at a glance
- **Create & edit invoices**: customer details, line items, discount %, tax %, notes, and due dates, with a live A4 preview
- **Invoice history**: search by customer or invoice number, filter by payment status (Pending / Paid / Overdue), and sort by date
- **View, edit, delete** any saved invoice, or mark it as paid
- **Print invoice**: clean A4 print layout; navigation and buttons are hidden when printing
- **Download PDF**: one-click PDF export (via jsPDF)
- **Automatic saving**: invoices are stored in `localStorage` and survive page refresh
- **Overdue detection**: unpaid invoices turn overdue after their due date
- **Form validation**: clear inline error messages
- **Responsive & accessible**: works on mobile, supports dark mode, keyboard friendly

## Getting started

No installation needed.

1. Download or clone this repository
2. Open `index.html` in your browser

```bash
git clone https://github.com/Haniabatool72/invoice-manager-app.git
cd invoice-manager-app
# then just open index.html
```

> The PDF download needs an internet connection (jsPDF is loaded from cdnjs). If it can't load, the app falls back to the print dialog, where you can choose "Save as PDF".

## Project structure

```
├── index.html   # Markup and views (dashboard, history, editor)
├── style.css    # Styles, A4 invoice layout, print rules
└── script.js    # App logic, localStorage, print and PDF
```

## Customize

Edit the `COMPANY` object at the top of the invoice section in `script.js` to set your own business name, address, email, phone and website.

## Tech stack

HTML5, CSS3, vanilla JavaScript, [jsPDF](https://github.com/parallax/jsPDF) + [jspdf-autotable](https://github.com/simonbengtsson/jsPDF-AutoTable)

## Notes

Data is stored per browser and device. Clearing site data removes saved invoices.

---

Developed by **Hania Batool**
