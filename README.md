# TodoList Frontend

A modern, responsive TodoList application built with React, TypeScript, and Tailwind CSS.

## Features

- ✅ **CRUD Operations** - Create, read, update, and delete todos
- 🎨 **Dark/Light Theme** - Toggle between dark and light modes
- 📱 **Mobile-First Design** - Responsive design for all devices
- 🔍 **Search & Filter** - Search todos and filter by priority, date, and completion status
- 📅 **Date Management** - Today and Upcoming views with date picker
- ♾️ **Infinite Scroll** - Lazy loading for better performance
- 🎯 **Priority Levels** - Low, Medium, and High priority todos
- 🚀 **Optimistic UI** - Instant feedback with TanStack Query

## Tech Stack

- **React 18** - UI library
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **TanStack Query** - Data fetching and caching
- **Redux Toolkit** - State management
- **shadcn/ui** - UI components
- **Day.js** - Date manipulation
- **Vite** - Build tool

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository

```bash
git clone <repository-url>
cd todolist-frontend
```

2. Install dependencies

```bash
npm install
```

3. Create environment file

```bash
cp .env.example .env.local
```

4. Update environment variables in `.env.local`

   **For local development:**

   - Keep `VITE_API_URL=http://localhost:8080` (uncommented)
   - Comment out the production URL

   **For production deployment:**

   - Comment out `VITE_API_URL=http://localhost:8080`
   - Uncomment `VITE_API_URL=https://backend-mvptodolistapp.onrender.com`

### Development

```bash
npm run dev
```

The app will start on `http://localhost:5173`

### Production Build

```bash
npm run build
npm run preview
```

## Environment Variables

| Variable        | Description      | Default                 |
| --------------- | ---------------- | ----------------------- |
| `VITE_API_URL`  | Backend API URL  | `http://localhost:8080` |
| `VITE_NODE_ENV` | Environment mode | `development`           |

## Deployment

This application is configured for deployment on Vercel.

### Vercel Deployment Steps

1. Connect your GitHub repository to Vercel
2. Set environment variables in Vercel dashboard
3. Deploy!

### Environment Variables for Production

Set these in your Vercel dashboard:

- `VITE_API_URL` = `https://your-backend-url.onrender.com`

## Project Structure

```
src/
├── components/          # React components
│   ├── ui/             # shadcn/ui components
│   └── ...
├── contexts/           # React contexts
├── hooks/              # Custom hooks
├── lib/                # Utilities and API client
├── store/              # Redux store and slices
├── types/              # TypeScript type definitions
└── main.tsx           # App entry point
```
