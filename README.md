# 💰 PriceLens

> A modern full-stack price tracking platform that helps users monitor products, analyze price trends, and receive instant alerts when prices drop.

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

## 📖 Overview

PriceLens is a modern web application that allows users to track product prices over time and receive notifications when prices drop.

Instead of manually checking products every day, users can simply paste a product URL and let PriceLens monitor it automatically. The application continuously tracks prices, stores historical data, and alerts users when a better deal becomes available.

## ✨ Key Features

* **Secure User Authentication:** Sign up and log in using email authentication powered by Supabase.
* **Product Tracking:** Add products instantly by pasting product URLs.
* **Automatic Product Extraction:** Fetches product name, current price, currency, and product image automatically.
* **Historical Price Monitoring:** Tracks price changes over time and maintains historical records.
* **Email Notifications:** Sends instant email alerts whenever a price drop is detected.
* **Personal Dashboard:** View and manage all tracked products from a centralized dashboard.
* **Responsive Design:** Optimized for desktop, tablet, and mobile devices.
* **Cloud Deployment:** Fully deployed and hosted on Vercel.

## 🏗️ System Architecture

1. **Frontend Layer:** Next.js App Router with React and Tailwind CSS provides a fast and responsive user interface.
2. **Authentication Layer:** Supabase Auth handles user registration and login securely.
3. **Product Scraping Layer:** Firecrawl API extracts product details directly from product pages.
4. **Database Layer:** Supabase stores product information, user accounts, and historical price data.
5. **Notification Layer:** Resend delivers automated email alerts when price drops occur.
6. **Deployment Layer:** Vercel hosts and serves the application globally.

## ⚙️ How It Works

1. User signs up or logs in using email authentication.
2. User pastes a product URL into the application.
3. PriceLens automatically extracts product information.
4. Product data is stored in the database.
5. Scheduled price checks compare current prices with previous values.
6. When a price drop is detected, an email notification is sent to the user.
7. Users can monitor all tracked products from their dashboard.

## 🛠️ Tech Stack

### Frontend
- Next.js (App Router)
- React
- Tailwind CSS

### Backend
- Next.js Server Actions
- Supabase

### Services
- Firecrawl API
- Resend
- Vercel

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- Supabase Project
- Firecrawl API Key
- Resend API Key

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/pricelens.git
cd pricelens
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env.local` file in the root directory:

```env
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
FIRECRAWL_API_KEY=your_firecrawl_api_key
RESEND_API_KEY=your_resend_api_key
```

### 4. Run the Development Server

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

## ☁️ Deployment

The application is deployed using Vercel.

### Deployment Steps

1. Push the project to GitHub.
2. Import the repository into Vercel.
3. Configure all environment variables.
4. Deploy the application.

## 🔒 Security Notes

- Environment variables are stored securely using `.env.local`.
- Sensitive credentials are never exposed to the client.
- Server-only operations are implemented using `"use server"`.
- Authentication and database access are managed through Supabase.

## 🔮 Future Improvements

- Browser Extension
- Progressive Web App (PWA)
- Telegram Notifications
- WhatsApp Notifications
- Advanced Price Analytics
- Multi-store Price Comparison

## 📌 Project Status

**Completed and Successfully Deployed**

## 👨‍💻 Author

**Prakhar Shakya**

Built with Next.js, Supabase, Firecrawl, Resend, and Vercel to help users make smarter purchasing decisions through automated price tracking.
