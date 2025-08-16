# Online Casino Gaming Platform

## Overview

This is a full-stack online casino gaming platform built with React and Express. The application features multiple casino games including Crash, Dice, and Slots, with real-time gameplay mechanics, user authentication, and virtual currency betting system. The platform provides a modern casino experience with responsive design and engaging user interfaces.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern development
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query for server state management and caching
- **UI Components**: Radix UI primitives with shadcn/ui component library for consistent design
- **Styling**: Tailwind CSS with custom casino theme variables and gradient utilities
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture
- **Runtime**: Node.js with Express.js framework for RESTful API endpoints
- **Language**: TypeScript for type safety across the full stack
- **Database ORM**: Drizzle ORM for type-safe database operations
- **Session Management**: Express sessions with PostgreSQL storage for user state persistence
- **Authentication**: Replit's OpenID Connect (OIDC) integration for secure user authentication
- **Development**: Hot module replacement and development middleware integration

### Data Storage Solutions
- **Primary Database**: PostgreSQL with connection pooling via Neon serverless driver
- **Session Storage**: PostgreSQL-backed session store for authentication state
- **Schema Management**: Drizzle Kit for database migrations and schema synchronization
- **Data Models**: Users, games, bets, game sessions, and transaction history tables

### Authentication and Authorization
- **Provider**: Replit OIDC for seamless authentication within the Replit ecosystem
- **Session Security**: HTTP-only cookies with secure flags and CSRF protection
- **User Management**: Automatic user creation and profile management with balance tracking
- **Route Protection**: Middleware-based authentication checks for sensitive endpoints

### Game Engine Architecture
- **Game Types**: Modular game implementations for Crash, Dice, and Slots
- **Random Number Generation**: Cryptographically secure RNG using Web Crypto API (client) and Node.js crypto module (server)
- **Fairness System**: Provably fair gaming with client/server seed combination for complete transparency
- **Real-time Mechanics**: Enhanced 3x3 slots with staggered reel animations and winning line detection
- **Betting System**: Decimal-based currency handling with server-side validation and transaction logging
- **Session Management**: Game state tracking and history for each game type

## External Dependencies

### Database and Infrastructure
- **Neon Database**: Serverless PostgreSQL hosting with connection pooling
- **WebSocket Support**: For potential real-time features via Neon's serverless infrastructure

### Authentication Services
- **Replit Identity**: OpenID Connect provider for user authentication and authorization
- **Passport.js**: Authentication middleware with OpenID Connect strategy support

### UI and Styling
- **Radix UI**: Comprehensive set of unstyled, accessible UI primitives
- **shadcn/ui**: Pre-built component library built on Radix UI foundations
- **Tailwind CSS**: Utility-first CSS framework with custom casino theme configuration
- **Lucide Icons**: Modern icon library for consistent iconography

### Development and Build Tools
- **Vite**: Next-generation frontend build tool with TypeScript support
- **Replit Integration**: Development environment plugins for seamless Replit workflow
- **ESBuild**: Fast JavaScript bundler for server-side code compilation

### Form and Data Management
- **React Hook Form**: Performant form library with validation support
- **Zod**: TypeScript-first schema validation for runtime type checking
- **TanStack Query**: Powerful data synchronization for server state management