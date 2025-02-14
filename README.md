# Banking Application

A modern financial SaaS platform built with Next.js that allows users to connect multiple bank accounts, view real-time transactions, and manage funds transfers between platform users.

## Features

- Secure SSR authentication with input validation
- Multiple bank account integration via Plaid
- Real-time transaction monitoring and updates
- Inter-account fund transfers using Dwolla
- Comprehensive transaction history with filtering
- Dashboard showing total balance, recent transactions, and spending categories
- Responsive design for all devices

## Tech Stack

- Next.js
- TypeScript
- Appwrite (Backend)
- Plaid (Banking Integration)
- Dwolla (Payment Processing)
- TailwindCSS
- React Hook Form
- Zod (Validation)
- Chart.js (Visualizations)
- ShadCN UI Components

## Setup Instructions

1. Configure environment variables in `.env`:
```env
#NEXT
NEXT_PUBLIC_SITE_URL=

#APPWRITE
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
APPWRITE_DATABASE_ID=
APPWRITE_USER_COLLECTION_ID=
APPWRITE_BANK_COLLECTION_ID=
APPWRITE_TRANSACTION_COLLECTION_ID=
APPWRITE_SECRET=

#PLAID
PLAID_CLIENT_ID=
PLAID_SECRET=
PLAID_ENV=sandbox
PLAID_PRODUCTS=auth,transactions,identity
PLAID_COUNTRY_CODES=US,CA

#DWOLLA
DWOLLA_KEY=
DWOLLA_SECRET=
DWOLLA_BASE_URL=https://api-sandbox.dwolla.com
DWOLLA_ENV=sandbox
```

2. Start the development server:
```bash
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Required External Services

You'll need to set up accounts with:
- [Appwrite](https://appwrite.io)
- [Plaid](https://plaid.com)
- [Dwolla](https://www.dwolla.com)
