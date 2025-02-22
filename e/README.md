<!-- # Secure Wallet Management System

A secure wallet management system for crypto, fiat, and RWA assets with mock integrations.

## Features

- User authentication
- Multi-wallet support (Crypto, Fiat, RWA, NFT)
- Digital asset management (NFTs and RWA tokens)
- Transaction history
- Secure key management

## Prerequisites

- Node.js (v18 or later)
- PostgreSQL database
- VS Code (recommended)

## Local Development Setup

1. Clone the repository:
```bash
git clone [your-repo-url]
cd [project-directory]
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with the following content:
```env
DATABASE_URL=postgresql://username:password@localhost:5432/your_database_name
```

4. Create and initialize the database:
```bash
npm run db:push
```

5. Start the development server:
```bash
npm run dev
```

The application will be available at http://localhost:5000

## Project Structure

```
├── client/                # Frontend React application
│   ├── src/
│   │   ├── components/   # Reusable UI components
│   │   ├── hooks/        # Custom React hooks
│   │   ├── lib/          # Utility functions
│   │   └── pages/        # Page components
├── server/               # Backend Express application
│   ├── auth.ts          # Authentication logic
│   ├── routes.ts        # API routes
│   └── storage.ts       # Database operations
└── shared/              # Shared code between frontend and backend
    └── schema.ts        # Database schema and types
```

## Database Schema

The application uses a PostgreSQL database with the following main tables:

- `users`: User accounts
- `wallets`: Wallet information
- `assets`: NFT and RWA token data
- `transactions`: Transaction history

## API Endpoints

### Authentication
- POST `/api/register` - Register new user
- POST `/api/login` - User login
- POST `/api/logout` - User logout
- GET `/api/user` - Get current user

### Wallets
- GET `/api/wallets` - List user's wallets
- GET `/api/wallets/:id` - Get wallet details
- POST `/api/wallets` - Create new wallet
- DELETE `/api/wallets/:id` - Delete wallet

### Assets
- GET `/api/wallets/:id/assets` - List wallet's assets
- POST `/api/wallets/:id/assets` - Add new asset

### Transactions
- GET `/api/wallets/:id/transactions` - Get wallet transactions

## Technology Stack

- Frontend: React, TanStack Query, Tailwind CSS, shadcn/ui
- Backend: Express.js, Passport.js
- Database: PostgreSQL with Drizzle ORM
- Build Tools: Vite, TypeScript

## Security Features

- Secure password hashing using scrypt
- Session-based authentication
- Encrypted private key storage
- CSRF protection -->


# Clone the repository (replace with actual repo URL)
git clone [repository-url]
cd [project-directory]

# Install all required dependencies
npm install @types/node @types/passport-local @types/express passport-local @radix-ui/react-tooltip @radix-ui/react-scroll-area @radix-ui/react-separator @neondatabase/serverless @radix-ui/react-slider tailwindcss @replit/vite-plugin-shadcn-theme-json framer-motion @radix-ui/react-checkbox @radix-ui/react-navigation-menu recharts @radix-ui/react-aspect-ratio ethers tsx postcss @radix-ui/react-accordion date-fns @vitejs/plugin-react typescript @radix-ui/react-slot esbuild @jridgewell/trace-mapping drizzle-kit @types/react tailwind-merge web3 @radix-ui/react-collapsible @radix-ui/react-radio-group @radix-ui/react-dialog clsx input-otp @radix-ui/react-toast @tanstack/react-query express-session zod-validation-error vaul @radix-ui/react-hover-card drizzle-zod class-variance-authority drizzle-orm connect-pg-simple ws @types/passport @radix-ui/react-switch @tailwindcss/typography @radix-ui/react-alert-dialog tailwindcss-animate express react passport @radix-ui/react-progress @replit/vite-plugin-runtime-error-modal @types/react-dom @radix-ui/react-toggle react-icons autoprefixer @types/express-session @radix-ui/react-context-menu memorystore cmdk zod @radix-ui/react-avatar @radix-ui/react-popover @radix-ui/react-tabs @hookform/resolvers lucide-react @radix-ui/react-dropdown-menu @radix-ui/react-menubar react-day-picker react-resizable-panels @radix-ui/react-label embla-carousel-react react-hook-form wouter @radix-ui/react-toggle-group vite @types/ws react-dom @radix-ui/react-select @types/connect-pg-simple

# Initialize the database schema
npm run db:push


npm run dev

