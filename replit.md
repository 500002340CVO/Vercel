# Antigua & Barbuda Tourism Website

## Overview

This is a modern tourism website for Antigua & Barbuda (known by the indigenous name "Wadadli"), showcasing the islands' beaches, culture, food, and attractions. The application features a React frontend with a clean, vibrant design inspired by Caribbean aesthetics, an Express.js backend with RESTful APIs, and an interactive chatbot for visitor assistance using local knowledge bases.

## User Preferences

Preferred communication style: Simple, everyday language.

## Recent Progress (January 7, 2025)
- ✅ Complete tourism website built with Caribbean-themed design
- ✅ Wadadli Bot chatbot integrated with local knowledge database 
- ✅ Vercel deployment configuration completed (vercel.json, api/chat.js)
- ✅ Deployment guides created (DEPLOYMENT.md, export-for-deployment.md)
- 🔄 User plans to continue deployment process tomorrow

## Next Steps
- Export project from Replit to GitHub
- Deploy to Vercel for free hosting with working chatbot
- Website will be publicly accessible at custom .vercel.app domain

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **Styling**: Tailwind CSS with custom Caribbean-themed color palette and shadcn/ui component library
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query for server state management and API caching
- **UI Components**: Radix UI primitives with custom styling for accessibility and consistency
- **Design System**: Component-based architecture with reusable UI elements and consistent theming

### Backend Architecture
- **Framework**: Express.js with TypeScript for RESTful API endpoints
- **Development Setup**: Hot reload with Vite integration for seamless development experience
- **Data Storage**: In-memory storage implementation with interface-based design for easy database migration
- **API Structure**: Clean separation between routes, storage, and business logic
- **Knowledge Base**: Local data structures for Antigua facts, FAQs, and tourism information

### Chatbot System
- **Implementation**: Custom chatbot with fuzzy string matching for question answering
- **Knowledge Sources**: Three main data sources - Antigua facts, general FAQs, and tourism Q&A
- **Search Algorithm**: Difflib-based closest match finding with configurable similarity thresholds
- **Response Logic**: Prioritized search through FAQ, then tourism Q&A, with fallback to random facts
- **Session Management**: UUID-based session tracking for conversation context

### Database Schema Design
- **ORM**: Drizzle ORM configured for PostgreSQL with type-safe database operations
- **Tables**: Users table for authentication and chat_messages table for conversation history
- **Schema Management**: Drizzle Kit for migrations and schema synchronization
- **Type Safety**: Full TypeScript integration with inferred types from database schema

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: PostgreSQL database driver optimized for serverless environments
- **drizzle-orm**: Type-safe ORM for database operations with PostgreSQL dialect
- **@tanstack/react-query**: Server state management and caching for React applications

### UI and Styling
- **@radix-ui/***: Complete set of accessible, unstyled UI primitives
- **tailwindcss**: Utility-first CSS framework with custom Caribbean color palette
- **class-variance-authority**: Type-safe utility for managing component variants
- **lucide-react**: Consistent icon library for user interface elements

### Development Tools
- **tsx**: TypeScript execution environment for Node.js development
- **esbuild**: Fast JavaScript bundler for production builds
- **@replit/vite-plugin-***: Replit-specific development tools and error handling
- **wouter**: Minimalist routing library for React applications

### Potential Database Integration
The application is configured to use PostgreSQL through Drizzle ORM, though currently using in-memory storage. The database configuration expects a `DATABASE_URL` environment variable and includes proper migration setup for production deployment.