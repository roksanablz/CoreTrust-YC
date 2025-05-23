# CoreTrust Dashboard

A comprehensive AI governance and risk management platform designed to help organizations understand and mitigate AI-related risks. Built with Next.js, TypeScript, and shadcn/ui.

## Overview

CoreTrust provides four main tools:

### 1. Dashboard
- Real-time model performance metrics
- Compliance status tracking
- Risk alerts and notifications
- System health monitoring

### 2. AI Tools Explorer
- Curated marketplace of vetted AI tools
- Risk assessment scores
- Compliance certifications
- Performance metrics

### 3. PolicySense™
- Global AI regulation tracking
- Real-time policy updates
- Impact assessment
- Implementation progress tracking

### 4. Risk Radar™
- Predictive risk assessment
- Case precedent analysis
- Actionable recommendations
- Risk trend monitoring

## Tech Stack

- Next.js 13+
- TypeScript
- Tailwind CSS
- shadcn/ui components

## Getting Started

### Prerequisites
- Node.js (v18 or newer)
- npm or yarn

### Installation
```bash
git clone https://github.com/roksanablz/CoreTrust-YC.git

cd CoreTrust-YC

npm install

npm run dev
```

Open http://localhost:3000 to view the platform

### Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
# Google Custom Search API credentials (required for policy scraping)
GOOGLE_API_KEY=your_google_api_key
GOOGLE_CSE_ID=your_custom_search_engine_id

# OpenAI API credentials (required for text analysis)
OPENAI_API_KEY=your_openai_api_key

# Congress.gov API credentials (required for legislative tracking)
CONGRESS_GOV_API_KEY=your_congress_gov_api_key
```

Note: The Congress.gov scraper uses web scraping and does not require an API key.

You can obtain these credentials from:
- Google Custom Search API: https://developers.google.com/custom-search/v1/overview
- OpenAI API: https://platform.openai.com/api-keys
- Congress.gov API: https://api.congress.gov/sign-up/

## Development

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npm run test` - Run tests

## Project Structure

- `/app` - Next.js app directory
- `/components` - React components
- `/lib` - Utility functions
- `/policy-crawler` - Policy analysis tools
- `/policy_scraper` - Python-based policy scraping tools

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT License

## Deployment

### Deploying to Vercel

1. Install Vercel CLI (optional):
```bash
npm install -g vercel
```

2. Deploy using one of these methods:

#### Method 1: Using Vercel Dashboard (Recommended)
1. Push your code to GitHub
2. Go to [Vercel Dashboard](https://vercel.com/dashboard)
3. Click "New Project"
4. Import your GitHub repository
5. Configure your environment variables (copy from your `.env` file)
6. Click "Deploy"

#### Method 2: Using Vercel CLI
1. Login to Vercel:
```bash
vercel login
```

2. Deploy the project:
```bash
vercel
```

3. Follow the CLI prompts to:
   - Set up and deploy
   - Configure environment variables
   - Choose your team and project name

The app will be automatically deployed and you'll receive a production URL.

### Environment Variables in Production

Make sure to add all your environment variables in the Vercel dashboard:
- `GOOGLE_API_KEY`
- `GOOGLE_CSE_ID`
- `OPENAI_API_KEY`
- `CONGRESS_GOV_API_KEY`

You can add these in:
1. Project Settings → Environment Variables
2. Add each variable with its corresponding value
3. Select the environments where they should be available (Production, Preview, Development)