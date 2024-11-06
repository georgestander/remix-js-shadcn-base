# Remix JS + shadcn/ui Starter

A minimal Remix starter template using JavaScript (no TypeScript) with shadcn/ui components and Tailwind CSS.

## What's included

- ✅ Remix (with Vite)
- ✅ JavaScript (no TypeScript)
- ✅ Tailwind CSS
- ✅ shadcn/ui components
- ✅ Pre-configured import aliases (~/)

## Getting Started

```bash
# Clone the repository
gh repo clone YOUR-USERNAME/remix-js-shadcn-base my-project-name
cd my-project-name

# Remove the old git history and start fresh
rm -rf .git
git init

# Install dependencies
npm install

# Start development server
npm run dev
Adding shadcn Components
bashCopy# Add any shadcn component you need
npx shadcn@latest add button
npx shadcn@latest add card
npx shadcn@latest add dialog
# etc...
Building for Production
bashCopy# Build the app
npm run build

# Start in production mode
npm start
Deployment
Built-in Remix app server is production-ready.
Deploy the output of npm run build:

build/server
build/client

Styling

Uses Tailwind CSS for styling
shadcn/ui components are pre-configured with CSS variables
Edit app/tailwind.css for global styles
Customize tailwind.config.js for theme settings