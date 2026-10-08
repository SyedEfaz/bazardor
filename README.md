# বাজার দর / BazarDor

A modern Bangla marketplace dashboard for tracking everyday grocery and household product prices across Bangladesh. The app helps users compare daily prices, discover category-wise trends, and manage their account profile.

## Overview

**Project name:** বাজার দর / BazarDor  
**Type:** Price tracking and market comparison web app  
**Audience:** Bangladesh consumers looking for daily market prices and trends

## Technologies used

- Next.js 15
- React 19
- TypeScript
- Tailwind CSS
- DaisyUI
- Better Auth
- MongoDB
- REST-based market data integration

## Key features

1. Daily market price overview for essential goods and groceries
2. Category-based browsing for rice, oil, vegetables, meat, fish, and more
3. Product detail pages with price range, average market value, and market comparisons
4. Price change tracking with up/down/flat indicators for trend analysis
5. User authentication, profile view, and profile information update support

## Setup

```powershell
npm install
Copy-Item .env.example .env
npm run dev
```

Configure the required environment variables in `.env`:

- `MONGODB_URI` — MongoDB connection string including database name
- `BETTER_AUTH_SECRET` — at least 32 characters
- `BETTER_AUTH_URL` — your app base URL
- `NEXT_PUBLIC_APP_URL` — frontend base URL
- OAuth credentials for Google, GitHub, and Discord if social sign-in is enabled

Example callback URLs:

- Google: `http://localhost:3000/api/auth/callback/google`
- GitHub: `http://localhost:3000/api/auth/callback/github`
- Discord: `http://localhost:3000/api/auth/callback/discord`

## Notes

- The app is designed for Bangla language users and uses Bangla-friendly formatting for prices and dates.
- The market data is fetched from external public price APIs and refreshed periodically.
- For production use, store your MongoDB connection and auth secrets in a secure environment manager or hosting platform.
