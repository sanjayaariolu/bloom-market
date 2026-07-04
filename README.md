
```markdown
# 🌸 BloomMarket - Premium Flower Delivery & Management System

BloomMarket is a modern, full-stack web application built with **Next.js** designed to connect flower dealers and customers. It features dynamic daily rates, time-gated ordering windows, automated billing, and a premium glassmorphism user interface.

## ✨ Features

### 🛒 For Customers
- **Time-Gated Ordering:** Customers can only place orders between **10:00 AM and 7:00 PM**.
- **Dynamic Pricing:** Prices are updated daily based on dealer submissions.
- **Lock-in Orders (TBD Pricing):** Customers can place orders even before the daily rates are published. The system automatically applies the correct price once the rate is finalized at noon.
- **Customer Dashboard:** Real-time visual charts showing 7-day spending history and today's market flower rates.
- **Auto-Invoicing:** Consolidated daily invoices are automatically generated for all orders placed during the day.

### 👑 For Admins
- **Powerful Dashboard:** Visual analytics showing revenue, order statuses, and top-selling flowers.
- **Manual Overrides:** Admins can manually update flower rates and edit invoice totals directly from the dashboard.
- **One-Click Invoice Generation:** Ability to manually trigger the daily invoice generation process.
- **Order & Customer Management:** Easily track customer details and update order statuses (Pending, Confirmed, Delivered).

### 🏪 For Dealers
- **Dealer Portal:** A dedicated portal for flower dealers to submit the next day's flower rates in advance.

### 🤖 Automation (Cron Jobs)
The system runs built-in background cron jobs via `node-cron`:
- **12:00 PM:** Automatically publishes pending dealer rates to the live storefront.
- **7:00 PM:** Automatically aggregates all customer orders for the day and generates official invoices.

## 💻 Tech Stack
- **Framework:** Next.js (App Router)
- **Frontend:** React, Vanilla CSS (Custom Glassmorphism UI)
- **Database:** Local File-based JSON storage (for simplicity and portability)
- **Automation:** `node-cron`
- **Design:** AI-generated 4K flower photography and premium UI/UX design.

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bloom-market.git
   cd bloom-market
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🔐 Demo Credentials
To access the Admin Dashboard, use the following credentials on the Login page:
- **Email:** `admin@flowerapp.com`
- **Password:** `admin123`

---
*Built with ❤️ for flower lovers.*
```
