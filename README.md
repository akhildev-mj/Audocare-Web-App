# Audocare AI Web App

A companion frontend for the **Audocare AI Voice Agent**, built using **Next.js** and **LiveKit SDK**. This web interface enables users to interact with the AI agent using voice and view real-time transcriptions of their conversation.

## 🧠 Overview

This web application connects to a LiveKit-powered voice agent backend and provides a minimal, voice-first interface for users. It supports:

* Real-time voice communication with the AI agent
* Display of transcriptions for each user utterance
* Notifications for agent availability
* React components for a smooth UX

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <>
cd audocare-ai-web-app
```

### 2. Install Dependencies

```bash
pnpm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory using the example file:

```bash
cp .env.example .env
```

Update it with your LiveKit credentials and other config values.

### 4. Run the Development Server

```bash
pnpm run dev
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

## 🔧 Available Scripts

* `pnpm run dev` - Start development server
* `pnpm run build` - Build for production
* `pnpm run start` - Start production server
* `pnpm run lint` - Lint the codebase
* `pnpm run format:check` - Check formatting using Prettier
* `pnpm run format:write` - Auto-format code

## 📁 Project Structure

| File / Folder                          | Description                                                      |
| ------------------------------------- | ---------------------------------------------------------------- |
| 📁 `app/`                              | Main application folder with pages, components, and hooks        |
| ├── 📁 `api/connection-details/`       | API route for establishing agent connection                      |
| │   └── `route.ts`                    | Handles backend communication setup                              |
| ├── 📁 `components/`                   | Reusable UI components                                           |
| │   ├── `CloseIcon.tsx`              | Close icon SVG component                                         |
| │   ├── `NoAgentNotification.tsx`    | Shows notification if agent is unavailable                       |
| │   └── `TranscriptionView.tsx`      | Displays real-time transcriptions                                |
| ├── 📁 `hooks/`                        | Custom React hooks                                               |
| │   ├── `useCombinedTranscriptions.ts`| Merges multiple transcription sources                            |
| │   └── `useLocalMicTrack.ts`        | Handles microphone audio track                                   |
| ├── `globals.css`                     | Global Tailwind + CSS styles                                     |
| ├── `layout.tsx`                      | Root layout component                                            |
| └── `page.tsx`                        | Main application entry page                                      |
| 📄 `.env`, `.env.example`             | Environment variable files                                       |
| 📄 `package.json`                     | Project metadata and scripts                                     |
| 📄 `tailwind.config.ts`              | Tailwind CSS configuration                                       |
| 📄 `postcss.config.mjs`              | PostCSS plugins configuration                                    |
| 📄 `next.config.mjs`                 | Next.js app configuration                                        |
| 📄 `tsconfig.json`                   | TypeScript compiler options                                      |
| 📄 `README.md`                       | Documentation for the web app                                    |

## 📆 Tech Stack

* **Framework**: Next.js 14
* **Styling**: Tailwind CSS
* **Voice & Media**: LiveKit SDK
* **Animations**: Framer Motion
* **Type Checking**: TypeScript

## ✅ Notable Features

* Clean, minimal interface for seamless user experience
* Fully customizable components
* Modular hooks for managing voice and transcription logic

## 📊 Future Improvements

* Theme support (light/dark mode)
* Enhanced error handling and session management
* Avatar integration for visual feedback

## ✨ Contributing

We welcome contributions to improve the app! Feel free to fork, submit PRs, or open issues.

---

Built with ♥ by the Audocare team.
