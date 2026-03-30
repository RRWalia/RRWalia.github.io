# Rupeewise Budget

A lightweight, fast, and intelligent personal finance app for tracking income and expenses—built with Indian users in mind. Manage UPI, cards, wallets, and cash all in one place, with AI-powered insights to help you save more.

## 🎯 Why I Built This

Managing money across multiple payment methods (UPI, credit cards, wallets, cash) is overwhelming. Most budgeting apps are bloated or don't feel right for Indian users. **Rupeewise Budget** is lean, mobile-first, and designed for daily use—add a transaction in seconds, see your cash flow instantly, and get smart suggestions about where you can save.

## ✨ Key Features

- **All-in-One Dashboard**
  - Track income, expenses, and savings in one view  
  - Monthly summary with clear income vs. expense breakdown  
  - Real-time budget status with over-budget alerts  

- **Smart Transaction Management**
  - Add, edit, and delete transactions with dates and notes  
  - Organized by category (Rent, EMI, Groceries, Fuel, Subscriptions, etc.)  
  - Recent transaction history at a glance  
  - Support for multiple transaction types  

- **Visual Analytics**
  - Pie chart showing expense breakdown by category  
  - Monthly savings trend visualization  
  - Progress bars for budget tracking  

- **AI-Powered Insights** ✨
  - Personalized money-saving tips  
  - Smart recommendations based on your spending patterns  
  - Real-time alerts when you're close to budget limits  

- **Budget Planning**
  - Set monthly budget targets  
  - Track budget usage percentage  
  - Get notified when over budget  

- **Mobile-First & Responsive**
  - Optimized for smartphone use  
  - Works seamlessly on desktop and tablet  
  - Clean, intuitive interface with no fluff  

- **Data Privacy First**
  - All data stored locally and securely  
  - No external tracking or ads  
  - You own your financial data  

## 🛠️ Tech Stack

**Frontend:**
- **React 18** – Fast, modern component framework  
- **Vite** – Lightning-fast build tool and dev server  
- **TypeScript** – Type-safe code for fewer bugs  
- **Tailwind CSS** – Utility-first styling  
- **Shadcn/ui** – High-quality, customizable UI components  

**State & Data Management:**
- **React Router v6** – Client-side routing  
- **React Hook Form** – Lightweight form handling  
- **TanStack React Query** – Server state and data fetching  
- **React Context API** – Shared state for transactions and budget  
- **Supabase** – Backend database and authentication  

**Visualizations & Interactions:**
- **Recharts** – Beautiful, responsive charts  
- **Framer Motion** – Smooth animations  
- **Radix UI** – Accessible component primitives  
- **Lucide React** – Clean icon library  

**Additional Tools:**
- **Zod** – Runtime schema validation  
- **Date-fns** – Date manipulation  
- **Sonner** – Toast notifications  
- **Vitest** – Unit and integration testing  
- **ESLint** – Code quality enforcement  

## 📁 Project Structure
rupeewise-budget/
├── src/
│ ├── components/ # Reusable UI components
│ │ ├── ui/ # Shadcn/ui primitives (buttons, dialogs, etc.)
│ │ ├── Header.tsx # App header
│ │ ├── AppLayout.tsx # Main layout wrapper
│ │ ├── AppSidebar.tsx # Desktop sidebar navigation
│ │ ├── BottomNav.tsx # Mobile bottom navigation
│ │ ├── SummaryCard.tsx # Income/Expense/Budget cards
│ │ ├── SpendingPieChart.tsx # Category breakdown chart
│ │ ├── SavingsTrendCard.tsx # Monthly savings trend
│ │ ├── AIInsightsCard.tsx # AI-powered tips
│ │ ├── RecentTransactions.tsx # Transaction list
│ │ ├── AddTransactionDialog.tsx# Add transaction modal
│ │ └── EditTransactionDialog.tsx# Edit transaction modal
│ │
│ ├── pages/ # Route pages
│ │ ├── Index.tsx # Dashboard home
│ │ ├── Transactions.tsx # Full transaction view
│ │ ├── Budget.tsx # Budget settings
│ │ └── Settings.tsx # App settings
│ │
│ ├── contexts/ # React Context for global state
│ │ ├── TransactionsContext.tsx # Shared transaction state
│ │ └── BudgetContext.tsx # Budget management state
│ │
│ ├── hooks/ # Custom React hooks
│ │ ├── useTransactions.ts # Transaction logic
│ │ ├── useBudget.ts # Budget calculations
│ │ └── use-mobile.ts # Mobile detection
│ │
│ ├── integrations/ # External service integrations
│ │ ├── supabase.ts # Database client setup
│ │ └── api.ts # API calls
│ │
│ ├── lib/ # Utility functions
│ │ └── utils.ts # Helper functions
│ │
│ ├── App.tsx # Root app component with routing
│ ├── App.css # Global styles
│ └── main.tsx # React DOM entry point
│
├── public/ # Static assets
├── supabase/ # Supabase migrations & config
├── test/ # Test files
├── vite.config.ts # Vite build configuration
├── tailwind.config.ts # Tailwind CSS theme
├── tsconfig.json # TypeScript configuration
├── eslint.config.mjs # Code quality rules
└── package.json # Dependencies & scripts

## 🚀 Getting Started

### Prerequisites

- **Node.js** 16+ and npm/yarn installed  
- **Git** for version control  
- **Supabase** account (free tier works great)  

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/RRWalia/rupeewise-budget.git
   cd rupeewise-budget
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env.local` file in the root directory:
   VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_anon_key


4. **Start the development server:**
```bash
npm run dev
```
The app will open at `http://localhost:5173`

### Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run build:dev    # Build in development mode
npm run preview      # Preview production build locally
npm run lint         # Run ESLint for code quality
npm run test         # Run tests once
npm run test:watch   # Run tests in watch mode
```

## 📊 How It Works

1. **Add Transactions** – Click the "+" button to add income or expenses with date, category, and notes.
2. **View Dashboard** – See monthly income, expenses, and savings at a glance.
3. **Check Analytics** – Pie charts and trends show where your money goes.
4. **Get AI Insights** – Personalized tips based on your spending patterns.
5. **Manage Budget** – Set a monthly budget and track your usage in real-time.

## 🎨 Design System

- **Colors:** Dark theme with accent colors for better readability  
- **Components:** Built with Shadcn/ui for consistency  
- **Icons:** Lucide React for clean, modern icons  
- **Animations:** Framer Motion for smooth transitions  
- **Responsive:** Mobile-first, works on all screen sizes  

## 🔒 Security & Privacy

- ✅ **No external tracking** – No analytics or third-party scripts  
- ✅ **Secure authentication** – Supabase for encrypted login  
- ✅ **Your data, your control** – Self-hosted or easily exportable  
- ✅ **HTTPS only** – All data transmitted securely  

## 🚦 Roadmap

- [ ] Multi-account support (personal, business, shared budgets)  
- [ ] Export to CSV and PDF  
- [ ] Goal-based savings tracker  
- [ ] Recurring transactions (subscriptions, EMI)  
- [ ] Receipt scanning with OCR  
- [ ] Optional cloud sync and backup  
- [ ] Budget comparison month-over-month  
- [ ] Dark mode refinements  

## 🤝 Contributing

This is a portfolio and learning project. I welcome feedback, bug reports, and small pull requests. If you have ideas for improvements:

1. Open an **Issue** to discuss the feature  
2. Fork the repo and create a feature branch  
3. Submit a **Pull Request** with a clear description  

## 📄 License

This project is licensed under the **MIT License** – feel free to use it as a starting point for your own budgeting app or personal finance project.

## 💡 Inspiration

Built with Indian users in mind, this app takes inspiration from:
- The need for fast, offline-first finance tracking  
- Common expense categories in the Indian context  
- A focus on savings over complex investment tracking  

## 📞 Connect

- **GitHub:** [@RRWalia](https://github.com/RRWalia)  
- **Portfolio:** Coming soon  

---

**Made with ❤️ for managing money smarter.**
