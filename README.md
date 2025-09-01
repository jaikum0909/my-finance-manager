# Frontend-My-Finance-Manager 

A modern React-based web application for managing personal finances, featuring AI-powered receipt scanning and interactive analytics.

---

## Features

- User Authentication – Secure registration and login system  
- Transaction Management – Add, edit, and delete income and expense records  
- Receipt Scanning – AI-powered PDF receipt processing via Google Gemini  
- Financial Analytics – Interactive charts and expense tracking reports  
- Budget Management – Create and monitor budgets by category  
- Responsive Design – Optimized for both desktop and mobile devices  
- Real-time Updates – Live transaction tracking and notifications  

---

## Tech Stack

- React 19.1.1 – Modern React with hooks and functional components  
- React Router 6.8.0 – Client-side routing  
- Axios 1.11.0 – API communication  
- Recharts 2.8.0 – Data visualization and charts  
- Sass 1.91.0 – CSS preprocessing  
- Date-fns 2.30.0 – Date utilities  
- React Testing Library & Jest – Testing framework  

---

## Prerequisites

Before running the frontend, ensure you have:

- Node.js v16+  
- npm or yarn installed  
- Backend API running at `http://localhost:8080`  

---

## Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd my-finance-manager-main/frontend
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Setup

This frontend is configured to proxy API requests to `http://localhost:8080`.
Ensure the backend is running before starting the frontend.

### 4. Run the Development Server

```bash
npm start
```

The app will be available at: `http://localhost:3000`

---

## Project Structure

```
src/
├── api/                    # API service modules
│   ├── auth.js             # Authentication endpoints
│   ├── axios.js            # Axios configuration
│   ├── budgets.js          # Budget API
│   ├── categories.js       # Category API
│   ├── expenses.js         # Expense API
│   ├── incomes.js          # Income API
│   └── transactions.js     # Transaction API
├── components/             # Reusable UI components
│   ├── auth/               # Authentication components
│   ├── charts/             # Data visualization components
│   ├── common/             # Shared UI components
│   ├── pagination/         # Pagination controls
│   ├── receipts/           # Receipt upload components
│   └── transactions/       # Transaction components
├── contexts/               # React Context providers
│   ├── AuthContext.js      # Authentication state management
│   └── TransactionContext.js # Transaction state management
├── hooks/                  # Custom React hooks
├── pages/                  # Application pages
├── utils/                  # Utility functions
└── assets/                 # Static assets and styles
```

---

## Available Scripts

* `npm start` – Run in development mode
* `npm test` – Launch the test runner
* `npm run build` – Build for production
* `npm run eject` – Eject CRA configuration

---

## Key Components

### Authentication

* LoginForm – User login with email and password
* RegisterForm – New user registration
* AuthContext – Global authentication state management

### Transactions

* TransactionForm – Add or edit income and expense transactions
* TransactionList – Display and manage transactions
* TransactionItem – Individual transaction display

### Analytics

* ExpenseByCategoryChart – Pie chart showing expenses by category
* ExpenseByDateChart – Line chart showing expenses over time
* IncomeVsExpenseChart – Bar chart comparing income and expenses

### Receipt Management

* ReceiptUploader – Upload and process PDF receipts
* PdfHistoryUploader – View and manage uploaded receipts

---
## Security Features

* JWT authentication
* Secure API communication
* Input validation and sanitization
* Protected routes and components
