# AI Chatbot with Google Gemini

A modern AI chatbot built with [Next.js](https://nextjs.org) 16, [Vercel AI SDK](https://sdk.vercel.ai/), and Google Gemini API. This project features a beautiful UI with AI-powered components and real-time streaming responses.

## Features

- 🤖 Powered by Google Gemini AI models via AI SDK
- ⚡ Real-time streaming responses
- 🎨 Modern UI with Radix UI components
- 🌊 Interactive flow diagrams with XYFlow
- 💬 Advanced chat interface with artifacts, code blocks, and more
- 🎯 Type-safe with TypeScript and Zod validation
- 🎨 Styled with Tailwind CSS 4

## Prerequisites

- Node.js 20.x or later
- A Google AI API key (get one from [Google AI Studio](https://aistudio.google.com/app/apikey))

## Getting Started

### 1. Clone and Install Dependencies

```bash
npm install
# or
pnpm install
# or
yarn install
```

### 2. Set Up Environment Variables

Create a `.env.local` file in the root directory and add your Google AI API key:

```bash
GOOGLE_GENERATIVE_AI_API_KEY=your_api_key_here
```

### 3. Run the Development Server

```bash
npm run dev
# or
pnpm dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the chatbot in action.

## Project Structure

```
my-chatbot/
├── app/
│   ├── api/chat/         # Chat API route with Gemini integration
│   ├── layout.tsx        # Root layout
│   └── page.tsx          # Main chat interface
├── components/
│   ├── ai-elements/      # AI-specific components (messages, artifacts, etc.)
│   └── ui/               # Reusable UI components (Radix UI)
├── lib/
│   └── utils.ts          # Utility functions
└── public/               # Static assets
```

## Key Technologies

- **[Next.js 16](https://nextjs.org)** - React framework with App Router
- **[Vercel AI SDK](https://sdk.vercel.ai/)** - AI streaming and hooks
- **[@ai-sdk/google](https://sdk.vercel.ai/providers/ai-sdk-providers/google-generative-ai)** - Google Gemini integration
- **[Radix UI](https://www.radix-ui.com/)** - Accessible component primitives
- **[Tailwind CSS 4](https://tailwindcss.com/)** - Utility-first CSS framework
- **[TypeScript](https://www.typescriptlang.org/)** - Type safety
- **[Zod](https://zod.dev/)** - Schema validation

## AI Components

This project includes a comprehensive set of AI-focused components:

- **Message** - Chat message display
- **Artifact** - Rich content artifacts
- **CodeBlock** - Syntax-highlighted code with Shiki
- **Canvas** - Visual canvas for AI interactions
- **ChainOfThought** - Reasoning visualization
- **ImageComponent** - AI-generated image display
- **Plan** - Task planning interface
- **Tool** - Tool usage display
- And many more...

## Learn More

### Next.js Resources
- [Next.js Documentation](https://nextjs.org/docs)
- [Learn Next.js](https://nextjs.org/learn)

### AI SDK Resources
- [Vercel AI SDK Documentation](https://sdk.vercel.ai/docs)
- [Google Gemini Provider](https://sdk.vercel.ai/providers/ai-sdk-providers/google-generative-ai)
- [AI SDK Examples](https://sdk.vercel.ai/examples)

### Google Gemini
- [Google AI Studio](https://aistudio.google.com/)
- [Gemini API Documentation](https://ai.google.dev/docs)

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme).

Remember to add your `GOOGLE_GENERATIVE_AI_API_KEY` environment variable in your Vercel project settings.

Check out the [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
