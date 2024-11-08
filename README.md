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
gh repo clone https://github.com/georgestander/remix-js-shadcn-base.git my-project-name 
cd my-project-name

# Remove the old git history and start fresh
rm -rf .git
git init

# Install dependencies
npm install

# Start development server
npm run dev
```

## Adding shadcn Components

```bash
# Add any shadcn component you need
npx shadcn@latest add button
npx shadcn@latest add card
npx shadcn@latest add dialog
# etc...
```

## Building for Production

```bash
# Build the app
npm run build

# Start in production mode
npm start
```

## Deployment

Built-in Remix app server is production-ready.
Deploy the output of `npm run build`:
- `build/server`
- `build/client`

## Styling

- Uses Tailwind CSS for styling
- shadcn/ui components are pre-configured with CSS variables
- Edit `app/tailwind.css` for global styles
- Customize `tailwind.config.js` for theme settings

## Official Documentation

For more information, refer to the official documentation:
- [Remix Quickstart](https://remix.run/docs/en/main/start/quickstart)
- [shadcn UI Documentation](https://ui.shadcn.com/docs)

## Warning
This project includes a temporary fix for a known vulnerability. The `@remix-run/server-runtime` package has been overridden to use `cookie` version `^0.7.2`. Please monitor the official repository for a permanent fix and update accordingly.

```json
"overrides": {
    "@remix-run/server-runtime": {
        "cookie": "^0.7.2"
    }
}
```