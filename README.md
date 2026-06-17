# Complete-business-management-system
A free, open source business management system.

v1.5
Here’s a complete feature list:

---

# 📊 Enterprise ERP System v1.5

**A fully offline, single‑file ERP solution** built with vanilla HTML, CSS, and JavaScript.  
No backend, no frameworks – just one `.html` file that runs in any modern browser.  
Data is stored securely in your browser’s `localStorage`.

---

## ✨ Key Highlights

- **Zero dependencies** (except two lightweight CDN libs for QR codes and PDFs)  
- **Material Design 3** light/dark theme with a customisable accent colour  
- **Fully responsive** – works on desktop, tablet, and mobile  
- **No sign‑up, no server** – everything stays on your machine  
- **Open source** – free for personal and commercial use  

---

## 📦 Modules & Features

### 📊 Dashboard
- Real‑time KPIs: total customers, active products, total revenue, paid, outstanding due, net profit, active employees, total purchased  
- Latest invoices snapshot  

### 👥 Customers (CRM)
- Personal & business info, addresses, custom fields  
- Customer type (retail, wholesale, VIP), source, industry  
- Financial tracking: credit limit, total spent, paid, due, loyalty points  
- Risk level and account status (active/inactive/blocked)  

### 📦 Products (Inventory)
- SKU, barcode, name, description, category, brand  
- **Comma‑separated size list** (e.g. `S,M,L,XL`)  
- Cost price, selling price, tax rate, discount  
- Stock management: quantity, reserved, available, reorder level, warehouse  
- Supplier linking  
- Active/inactive/discontinued status  

### 🧾 Invoices
- Multi‑item invoices with **dynamic size dropdown**  
  - Select a product → auto‑populates sizes from its inventory  
  - Choose a pre‑defined size or select **“Others”** to type a custom size  
- Auto‑fill customer details (name, phone, email, address)  
- Seller selection with quick‑add employee  
- Payment method, paid amount, transaction ID, due date  
- Promo code integration (auto‑applies discount from Offers)  
- Custom note & terms & conditions (checkbox)  
- Company logo upload (Base64 stored)  
- **QR code** embedding on invoice  
- **Print** invoice (optimised printable window)  
- **Email invoice as PDF** (downloads PDF, opens mail client)  
- Automatic stock deduction when issued/paid  
- Status tracking: draft → issued → partial → paid  

### 💰 Sales
- Automatically generated from invoices when issued/paid  
- Links to employee/seller for performance tracking  
- Profit calculation (sale price minus cost price)  

### 🏦 Finance
- Income entries (auto‑populated from invoices + manual)  
- Expense entries with categories and notes  
- Net profit calculation displayed as KPI  

### 👷 Employees (HRM)
- Personal details, NID, father/mother name, address  
- Job info: department, role (dropdown with custom option), salary, join date  
- Attendance & payroll placeholders  
- Sales‑by‑employee report (total sales, count, last sale date)  

### 🚚 Suppliers
- Name, company, phone, email, address  
- Payment terms, rating  
- Link to products and purchases  

### 📥 Purchases
- Multiple items with size (datalist from product inventory)  
- Quantity, unit cost, payment method, transaction ID  
- **Stock auto‑increase** when purchase completed  
- **Print purchase order**  

### 📬 Deliveries (Courier)
- Linked to an invoice  
- Delivery address, status (pending, shipped, delivered), cost  

### 🏷️ Offers & Promos
- Promo name, code, type (percentage or fixed amount)  
- Optional product filter  
- Start & expiry dates  
- Active/inactive status  
- **Auto‑applied** in invoices when code selected  

### 🤖 AI Advisor
- Scans for low‑stock products and overdue invoices  
- Shows actionable alerts with one‑click buttons:  
  - **Call supplier** / **Email supplier** for low stock  
  - **Quick create purchase order**  
  - **Call customer** / **Email customer** for overdue invoices  
  - **View invoice**  

### 📈 Reports
- Revenue, profit, expenses KPIs  
- **Canvas‑drawn pie chart** overview  
- **Generate daily report** saved to history  

### ⚙️ Settings
- Company name, address, phone, currency, country  
- Light/dark theme toggle + custom accent colour  
- **Import / Export all data** as JSON (full backup)  
- **Clear all data** with confirmation  
- Silent auto‑export every 5 minutes  

### 🔔 Alerts & Notifications
- Bell icon with badge count  
- Alerts for low stock, overdue invoices, shipments in transit  
- **Sound** when new alerts appear  
- Modal with detailed alert list  

---

## 🎨 UI/UX
- Material Design 3 components (cards, buttons, badges)  
- Smooth sidebar navigation with 14 panels  
- Modal dialogs for all CRUD operations  
- Inline search & date filtering on all tables  
- Table sorting (numeric, text, and **smart date sorting**)  
- Responsive sidebar (overlay on mobile)  
- Escape key closes modals  
- Toast notifications  
- Live clock in top bar  

---

## 🛡️ Security & Stability
- **All dynamic content sanitised** (XSS protection)  
- Data saved immediately on every change  
- `beforeunload` warning if unsaved  
- Canvas charts draw only when visible (avoid rendering errors)  
- Date filters and sorts use ISO format for reliability  

---

## 📁 Technical Specs
|                     |                                           |
|---------------------|-------------------------------------------|
| **File size**       | ~ 55 KB (single HTML file)                |
| **Browser support** | Chrome, Firefox, Edge, Safari (modern)    |
| **External libs**   | `qrcodejs` (QR), `html2pdf.js` (PDF) – loaded from CDN |
| **Storage**         | `localStorage` with key prefix `erp_`     |
| **License**         | Open Source (MIT)                         |

---

## 🚀 How to Use
1. Download the `erp.html` file  
2. Open it in any modern browser  
3. Start adding customers, products, invoices…  
4. Export your data regularly as a backup  

---

## 🧑‍💻 Credits
- **Developed by:** AI  
- **Instructed & Constructed by:** MD. JUNAYED AL HABIB  
- **YouTube:** [@iamxtremeV](https://www.youtube.com/@iamxtremeV)  

---

Perfect for small businesses, freelancers, or as a learning resource for full‑stack frontend development.  
No installation, no cost, no limits.
