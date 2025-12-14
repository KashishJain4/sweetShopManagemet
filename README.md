# 🍭 Sweet Shop API Backend






## ⚡ Crafting Tools

Crafted using TypeScript, Express, Python, FastAPI, Jest and Pytest for TDD, LangChain/LangGraph, OpenAI, React, NextJS, Docker, Containerization, VPS(DigitalOcean), GitHub Workflows:
- **Backend**: TypeScript, Express.js, Node.js
- **Database**: MongoDB with Mongoose ODM
- **Testing**: Jest, Supertest (TDD approach)
- **AI/ML**: LangChain, LangGraph, OpenAI APIs
- **DevOps**: Docker, Containerization
- **Deployment**: VPS (DigitalOcean), GitHub Workflows for Test Checking
- **Package Manager**: pnpm
---
- **AI Framework**: LangChain, LangGraph for agent orchestration
- **Language Model**: OpenAI GPT-4 for natural language understanding
- **Backend**: FastAPI, Python 3.11
- **Memory**: Redis for chat history and session management
- **Database**: MongoDB integration for sweet inventory access
- **Testing**: Pytest with comprehensive test coverage
- **Package Manager**: pip with requirements.txt
---
- **Frontend**: Next.js 15, React 19, TypeScript
- **Styling**: TailwindCSS v4, Radix UI components
- **State Management**: Zustand for global state, React Query for server state
- **Forms**: React Hook Form with Zod validation
- **UI Components**: Custom components built with Radix UI primitives
- **Icons**: Lucide React icons
- **Package Manager**: pnpm

## 📊 Test Coverage

![Test Coverage](./public/test-coverage.png)

This project follows **Test-Driven Development (TDD)** principles with comprehensive test coverage:
- ✅ **80%+ Test Coverage**
- 🔍 **Unit Tests** for all controllers
- 🌐 **Integration Tests** for API endpoints
- 🏃‍♂️ **Continuous Testing** with GitHub Actions

### 🧪 TDD Implementation Evidence
All features were implemented following the **Red-Green-Refactor** cycle:
1. ❌ **Red**: Write failing tests first
2. ✅ **Green**: Write minimal code to pass tests  
3. 🔄 **Refactor**: Improve code while keeping tests passing

### 📋 Latest Test Results
```bash
All files: 80% Statements (144/180), 81.81% Branches (54/66), 80.76% Functions (21/26), 79.48% Lines (124/156)

Coverage Breakdown by Directory:
├── src/controllers/     100% coverage (97/97 statements)
├── src/models/         100% coverage (5/5 statements)  
├── src/routes/         100% coverage (11/11 statements)
├── src/test-utils/     100% coverage (21/21 statements)
├── src/config/         0% coverage (0/10 statements)
└── src/                27.77% coverage (10/36 statements)
```

## 🛠️ Features

### Core Functionality
- 🍬 **Sweet Management**: Add, view, update, delete sweets
- 🔍 **Advanced Search**: Filter by name, category, price range
- 📦 **Inventory Management**: Purchase and restock operations
- 🏷️ **Category Management**: Dynamic category listing
- 📈 **Real-time Stock Updates**: Automatic quantity management
- 🤖 **AI Waiter Chatbot**: Natural language interaction for product details and direct purchases through our intelligent AI assistant

### API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/add` | Add a new sweet to inventory |
| `GET` | `/view-all` | Get all sweets |
| `DELETE` | `/delete/:id` | Remove sweet from inventory |
| `GET` | `/search` | Search sweets with filters |
| `POST` | `/purchase/:id` | Purchase sweet (reduce quantity) |
| `POST` | `/restock/:id` | Restock sweet (increase quantity) |
| `GET` | `/categories` | Get all unique categories |

## 🚀 Quick Start

### Prerequisites
- **Node.js** (v16 or higher)
- **MongoDB** (local or cloud)
- **pnpm** package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vinitborad/incubyte-project-backend.git
   cd incubyte-project-backend
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   ```
   Update `.env` with your configuration:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://127.0.0.1:27017/sweet-shop
   NODE_ENV=development
   ```

4. **Start the application**
   ```bash   
   # Production build
   pnpm build
   pnpm start
   ```

### 🧪 Running Tests

```bash
# Run all tests
pnpm test

# Run tests with coverage
pnpm test:coverage

# Watch mode for development
pnpm test --watch
```

## 🐳 Docker Deployment

This project includes a multi-stage Dockerfile for optimized production deployment:

```bash
# Build the image
docker build -t sweet-shop-backend .

# Run the container
docker run -p 5000:5000 --env-file .env sweet-shop-backend
```

### Multi-stage Build Benefits
- 📦 **Smaller Image Size**
- 🔒 **No dev dependencies in production**
- ⚡ **Fast Startup: Optimized for cloud deployment**

## 📁 Project Structure

```
backend/
├── src/
│   ├── config/
│   │   └── db.ts                 # Database configuration
│   ├── controllers/
│   │   ├── sweet.controller.ts   # Business logic
│   │   └── sweet.controller.test.ts # Controller tests
│   ├── models/
│   │   ├── sweet.model.ts        # Mongoose model
│   │   └── sweet.schema.ts       # Data schema & validation
│   ├── routes/
│   │   └── sweet.routes.ts       # API routes definition
│   ├── test-utils/
│   │   └── db-handler.ts         # Test database utilities
│   ├── app.ts                    # Express app configuration
│   ├── server.ts                 # Server entry point
│   └── check-env.ts              # Environment validation
├── coverage/                     # Test coverage reports
├── public/
│   └── test-coverage.png         # Coverage visualization
├── Dockerfile                    # Multi-stage production build
├── jest.config.js               # Jest testing configuration
├── tsconfig.json                # TypeScript configuration
└── README.md                    # You are here! 📍
```

## 🚢 Deployment

### VPS Deployment (DigitalOcean)
This application is deployed on a VPS with:
- 🐳 Docker containerization
- 🔄 GitHub Actions CI/CD
- 🌐 Nginx reverse proxy
- 🔒 SSL/TLS encryption

##  Future Enhancements

Given more time, I would love to extend this project with:
- 🔐 **Authentication & Authorization** (Role-based access)
- 📧 **Email Notifications** for low stock alerts
- 📊 **Analytics Dashboard** with sales insights
- 🛒 **Shopping Cart** functionality
- 💳 **Payment Integration** (Stripe/Razorpay)
- 📱 **Mobile App** with React Native
- 🔍 **Advanced Search** with Elasticsearch
- 📈 **Real-time Analytics** with WebSockets






</div>
