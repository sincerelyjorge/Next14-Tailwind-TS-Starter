# PromptMeme Product Requirements Document (PRD)

## 1. Project Overview

**PromptMeme** is a fun and casual web app where users can quickly generate and share AI-created visual content. Designed for instant creativity and social engagement, the app provides a playful space for users to create memes, art, and other visuals using AI prompts. With a focus on simplicity, fast sharing, and viral appeal, PromptMeme is perfect for those seeking lighthearted, visually-driven interactions.

## 2. Core Functionalities

### 2.1 Browse
* User can view user-generated memes and trending content
* User can explore popular (liked) memes and view categorized collections
* Advanced search functionality by topic, keyword, phrase, and hashtags
* Personalized feed customization through user/topic following
* Robust content moderation system with NSFW filtering
* Smooth browsing experience with pagination or infinite scroll

### 2.2 Engage
* Interactive reactions including likes and moderation flagging
* Multi-channel sharing capabilities across SMS, social media, and email
* Content remixing tools for creative reimagining
* Detailed analytics dashboard for creators to track performance

### 2.3 Create
* AI-powered content generation using:
  * DALL-E for image creation
  * GPT-4 for message generation
  * ElevenLabs, Suno AI, and SoundDraw for audio elements
* Text overlay and editing capabilities
* Remix functionality for existing content
* Draft system for work-in-progress content

## 3. Technical Infrastructure Needs
* Rate limiting for AI generation requests
* Optimized image handling with caching
* CDN integration for content delivery
* Webhook notification system
* Queue management for AI tasks
* Comprehensive error handling
* Mobile-first responsive design
* PWA implementation

## 4. User Experience
* Streamlined onboarding process
* Interactive tutorial system
* Generation history tracking
* Favorite/Recent prompt management
* Efficient sharing mechanisms
* Preview functionality
* Undo/Redo system

## 5. Documentation References
* OpenAI: https://platform.openai.com/docs/api-reference/introduction
* ElevenLabs: https://help.elevenlabs.io/hc/en-us/sections/14163158308369-API
* Suno API via PiAPI: https://piapi.ai/suno-api
* SoundDraw: https://docs.google.com/document/d/185WjC7T1Rq1-9zKlARobmeFiR3VaJcN1IT4ZwDP03Tg/edit?pli=1&tab=t.0#heading=h.3pt5vjbx3xdc

## 6. File Structure
├── README.md
├── app
│   ├── favicon.ico
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components
│   └── ui
│       ├── accordion.tsx
│       ├── aspect-ratio.tsx
│       ├── avatar.tsx
│       ├── button.tsx
│       ├── card.tsx
│       ├── carousel.tsx
│       ├── checkbox.tsx
│       ├── dialog.tsx
│       ├── drawer.tsx
│       ├── dropdown-menu.tsx
│       ├── hover-card.tsx
│       ├── input.tsx
│       ├── label.tsx
│       ├── menubar.tsx
│       ├── pagination.tsx
│       ├── progress.tsx
│       ├── resizable.tsx
│       ├── scroll-area.tsx
│       ├── select.tsx
│       ├── separator.tsx
│       ├── sheet.tsx
│       ├── sidebar.tsx
│       ├── skeleton.tsx
│       ├── textarea.tsx
│       └── tooltip.tsx
├── components.json
├── eslint.config.mjs
├── hooks
│   └── use-mobile.tsx
├── instructions
│   └── instructions.md
├── lib
│   └── utils.ts
├── next-env.d.ts
├── next.config.ts
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── public
│   ├── file.svg
│   ├── globe.svg
│   ├── next.svg
│   ├── vercel.svg
│   └── window.svg
├── tailwind.config.ts
└── tsconfig.json

## 7. Additional Requirements

### 7.1 Project Setup
* Component organization in root /components directory
* Page routing through Next.js 14 app router
* Server-side data fetching with prop passing
* Client components marked with 'use client'

### 7.2 Server-side API Calls
* External API interactions handled server-side
* Dedicated API routes for each integration
* Client-side data fetching through internal API routes

### 7.3 Environment Variables
* Secure credential management
* Local development configuration
* Production environment setup
* Server-side-only access

### 7.4 Error Handling and Logging
* Comprehensive error management
* Server-side logging
* User-friendly error display

### 7.5 Type Safety
* TypeScript interface implementation
* Strict typing enforcement

### 7.6 Data Fetching in Components
* React hook implementation
* Loading state management
* Error handling integration

### 7.7 Fonts
* Tailwind-based font management

## 8. Core Stack
* Next.js 14 (with App Router)
* TypeScript
* Tailwind CSS

## 9. Authentication
* Clerk

## 10. Database
* Supabase

## 11. UI Components
* shadcn/ui
* Lucide Icons

## 12. Image Generation
* OpenAI (DALL-E)

## 13. Email
* Resend.com

## 14. Deployment
* Vercel

## 15. Development Tools
* ESLint
* Prettier