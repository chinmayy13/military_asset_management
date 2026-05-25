# Military Asset Management System

A full-stack web application designed to manage military assets, equipment transfers, personnel assignments, and purchases across multiple bases. Built using React, Node.js, Express, and PostgreSQL.

---

## Features

### Asset Management
- Track military equipment across different bases
- Monitor asset quantities and availability in real time
- Maintain organized records of purchases and transfers

### Personnel Management
- Assign personnel to specific bases and roles
- Manage assignment history efficiently

### Authentication & Security
- Secure login and registration system
- JWT-based authentication
- Role-based access control
- Password encryption using bcrypt

### Dashboard & Analytics
- Interactive dashboard with important metrics
- Charts and visual reports for better monitoring
- Responsive design for desktop and mobile devices

---

## Tech Stack

### Frontend
- React 18
- TypeScript
- Tailwind CSS
- React Router
- Recharts
- Vite

### Backend
- Node.js
- Express.js
- PostgreSQL
- JWT Authentication
- bcryptjs
- CORS

### Development Tools
- ESLint
- Nodemon
- Concurrently

---

## Getting Started

### Prerequisites
Make sure the following are installed on your system:

- Node.js (v18 or above)
- PostgreSQL
- npm or yarn

---

## Installation

### 1. Clone the Repository

```bash
git clone <repository-url>
cd military-asset-management
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Variables

Create a `.env` file in the root directory and add:

```env
NODE_ENV=development

DB_HOST=your-database-host
DB_PORT=5432
DB_NAME=your-database-name
DB_USER=your-database-user
DB_PASSWORD=your-database-password

JWT_SECRET=your-secret-key

PORT=3000

VITE_API_BASE_URL=http://localhost:3000
```

---

## Database Setup

- Make sure PostgreSQL is running
- Create a database for the project
- Tables will be created automatically on first run

---

## Running the Project

### Development Mode

Run frontend and backend together:

```bash
npm run dev:full
```

Or run separately:

```bash
npm run dev      # Frontend
npm run server   # Backend
```

---

### Production Build

```bash
npm run build
npm start
```

---

## Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start frontend server |
| `npm run server` | Start backend server |
| `npm run dev:full` | Run frontend + backend together |
| `npm run build` | Create production build |
| `npm start` | Start production server |
| `npm run lint` | Run ESLint |

---

## Main Database Tables

- `users`
- `bases`
- `equipment_types`
- `purchases`
- `transfers`
- `assignments`
- `asset_balances`

---

## API Routes

### Authentication
- `POST /auth/login`
- `POST /auth/signup`
- `GET /auth/verify`

### Assets & Transfers
- `GET /assets`
- `POST /purchases`
- `GET /purchases`
- `POST /transfers`
- `GET /transfers`

### Personnel
- `POST /assignments`
- `GET /assignments`

---

## Deployment

The project can be deployed easily on platforms like Render or Railway with PostgreSQL support.

---

## Future Improvements

- Asset maintenance tracking
- Notification system
- Advanced analytics dashboard
- Audit logs
- Multi-role admin panel

