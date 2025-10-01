# X Clone - Social Media Platform

A modern social media platform inspired by X (formerly Twitter), featuring real-time posts, user interactions, and advanced social networking capabilities.

## Features

- 📝 **Real-time Posts** - Share and discover content in real-time
- 👥 **User Profiles** - Complete user profile management
- 💬 **Interactions** - Like, comment, and share functionality
- 🔍 **Advanced Search** - Find users and content easily
- 🔔 **Notifications** - Real-time notification system
- 📱 **Responsive Design** - Optimized for all devices
- ⚡ **Performance** - Fast loading and smooth interactions

## Tech Stack

- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Modern styling framework
- **Prisma** - Database ORM
- **NextAuth.js** - Authentication
- **Socket.io** - Real-time communication
- **UploadThing** - File upload service

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn or pnpm

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd x-clone
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Set up environment variables:
```bash
cp .env.example .env.local
# Edit .env.local with your configuration
```

4. Set up the database:
```bash
npx prisma generate
npx prisma db push
```

5. Start the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

6. Open your browser and navigate to `http://localhost:3000`

## Environment Variables

Create a `.env.local` file with:
```env
# Database
DATABASE_URL="your_database_url"

# Authentication
NEXTAUTH_SECRET="your_nextauth_secret"
NEXTAUTH_URL="http://localhost:3000"

# OAuth Providers (optional)
GOOGLE_CLIENT_ID="your_google_client_id"
GOOGLE_CLIENT_SECRET="your_google_client_secret"
GITHUB_CLIENT_ID="your_github_client_id"
GITHUB_CLIENT_SECRET="your_github_client_secret"

# File Upload
UPLOADTHING_SECRET="your_uploadthing_secret"
UPLOADTHING_APP_ID="your_uploadthing_app_id"
```

## Building for Production

```bash
npm run build
# or
yarn build
# or
pnpm build
```

## Deployment

The application can be deployed to Vercel, Netlify, or any other hosting platform that supports Next.js applications.

## License

MIT License