# 📊 Fintraa - Financial Analytics Platform

> A powerful full-stack financial analytics platform that transforms complex financial data into actionable insights, built with modern web technologies and real-time visualization capabilities.

![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

## ✨ Features

### 📈 Advanced Analytics Dashboard
- **Real-time Visualization**: Interactive charts and graphs powered by Recharts
- **Customizable Layouts**: Flexible dashboard configurations for different use cases
- **Data Analysis**: Comprehensive user statistics and trend analysis
- **Performance Metrics**: Track key financial indicators and performance metrics
- **Responsive Design**: Fully responsive layouts that work on all devices

### 👥 User Management & Security
- **Secure Authentication**: Powered by Clerk with multi-factor authentication
- **Role-based Access**: Granular control over user permissions and access levels
- **User Verification**: Built-in verification system for account security
- **Activity Tracking**: Detailed logs of user actions and system changes
- **Session Management**: Secure session handling and token-based authentication

### 💼 Enterprise Features
- **Multi-company Support**: Manage multiple organizations from a single platform
- **Custom Tables**: Create and manage custom data structures
- **Data Import/Export**: Support for various data formats (CSV, JSON)
- **Company Analytics**: Organization-specific dashboards and reports
- **Audit Trails**: Track all changes and modifications within the system

### 🛠️ Technical Features
- **Modern UI Components**: Built with Radix UI primitives
- **Theme Support**: Light/dark mode with next-themes
- **Form Handling**: Powered by react-hook-form with validation
- **State Management**: React Query for efficient data fetching
- **Animations**: Smooth transitions with Framer Motion
- **Toast Notifications**: User-friendly notifications with Sonner
- **Date Handling**: Comprehensive date utilities with date-fns
- **Data Grid**: Advanced data manipulation with react-data-grid
- **Icons**: Rich icon set from @tabler/icons-react and lucide-react

## 🏗️ Project Structure

### 📱 Client (Frontend)
```
client/
├── src/
│   ├── app/                    # Next.js app directory
│   │   ├── (auth)/            # Authentication pages
│   │   ├── (main)/            # Main application routes
│   │   │   ├── dashboard/     # Dashboard components
│   │   │   ├── settings/      # User settings
│   │   │   └── analytics/     # Analytics features
│   │   └── api/              # API routes
│   ├── components/
│   │   ├── ui/               # Reusable UI components
│   │   ├── forms/            # Form components
│   │   └── charts/           # Chart components
│   ├── lib/                  # Utility functions
│   ├── hooks/                # Custom React hooks
│   └── styles/               # Global styles
```

### ⚙️ Server (Backend)
```
server/
├── controller/              # Business logic
│   ├── userController.js    # User management
│   ├── companyController.js # Company operations
│   └── analyticsController.js # Analytics processing
├── model/                  # MongoDB schemas
├── routes/                 # API endpoints
├── middleware/             # Custom middleware
│   ├── auth.js            # Authentication
│   └── validation.js      # Request validation
├── db/                    # Database configuration
├── utils/                 # Helper functions
└── webhooks/              # Webhook handlers
```

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ installed
- MongoDB 6.0+ database
- Clerk account for authentication
- npm 9+ or yarn 1.22+
- Git for version control

### Frontend Setup
```bash
cd client
npm install
npm run dev
```
Visit [https://fintraa.vercel.app/](https://fintraa.vercel.app/) to see the live application.

### Backend Setup
```bash
cd server
npm install
npm run dev  # For development with auto-reload
# or
npm start    # For production
```

## 🔧 Environment Variables

### Frontend (.env)
```env
# Authentication (Required)
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# API Configuration (Required)
NEXT_PUBLIC_API_URL=your_api_url

# Feature Flags (Optional)
NEXT_PUBLIC_ENABLE_ANALYTICS=true
NEXT_PUBLIC_ENABLE_NOTIFICATIONS=true
```

### Backend (.env)
```env
# Database (Required)
MONGODB_URI=your_mongodb_uri

# Server Configuration (Required)
PORT=3001
NODE_ENV=development

# Authentication (Required)
CLERK_SECRET_KEY=your_clerk_secret

# Security (Optional)
CORS_ORIGIN=https://fintraa.vercel.app
RATE_LIMIT_WINDOW=15
RATE_LIMIT_MAX=100
```

## 💻 Development

### Key Technologies & Versions
- **Frontend**:
  - Next.js 14.2.15
  - React 18
  - TypeScript 5
  - Tailwind CSS 3
  - Clerk Authentication
  - Recharts 2.13
  - React Query 5
  - React Hook Form 7
  - Radix UI Components
  - Framer Motion 11

- **Backend**:
  - Node.js 18+
  - Express 4.21
  - MongoDB with Mongoose 8.7
  - JWT Authentication
  - Clerk SDK 5.0
  - CORS enabled
  - Express Async Handler

### Code Style & Quality
- ESLint for code linting
- Prettier for code formatting
- TypeScript strict mode
- Husky for pre-commit hooks
- Jest for testing
- GitHub Actions for CI/CD

## 📦 Deployment

### Frontend Deployment
1. Build the Next.js application:
```bash
cd client
npm run build
```
2. Deploy to Vercel:
   - Connect your GitHub repository
   - Configure environment variables
   - Enable automatic deployments

### Backend Deployment
1. Prepare for production:
   - Set up environment variables
   - Configure MongoDB connection
   - Set up logging and monitoring
2. Deploy to your preferred hosting:
   - Vercel
   - Railway
   - Heroku
   - AWS/GCP/Azure

## 📚 Documentation

- [Next.js Documentation](https://nextjs.org/docs)
- [Express.js Guide](https://expressjs.com)
- [Clerk Authentication](https://clerk.com/docs)
- [Recharts API](https://recharts.org/en-US/api)
- [React Query Guide](https://tanstack.com/query/latest)
- [Mongoose Documentation](https://mongoosejs.com/docs/guide.html)



## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Thanks to all contributors who have helped shape Fintraa
- Built with modern open-source technologies
- Inspired by the need for better financial analytics tools

---

<div align="center">

### 🌟 Fintraa - Making Financial Analytics Simple

[Website](https://fintraa.vercel.app/) · [Documentation](https://github.com/nabinhamal/fintra) · [Report Bug](https://github.com/nabinhamal/fintra) · [Request Feature](https://github.com/nabinhamal/fintra)

Made with ❤️ by the Fintraa Team
</div>

