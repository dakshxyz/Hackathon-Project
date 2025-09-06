# EcoFinds - Sustainable Second-Hand Marketplace

## Overview

EcoFinds is a full-stack sustainable second-hand marketplace application that enables users to buy and sell pre-owned items. The platform focuses on promoting environmental sustainability by facilitating the reuse of goods. Users can browse products, manage their own listings, add items to a shopping cart, and complete purchases. The application emphasizes a clean, user-friendly experience with features like search and filtering, user authentication, and order management.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **Routing**: Client-side routing implemented with Wouter for lightweight navigation
- **UI Framework**: Shadcn/ui component library built on top of Radix UI primitives
- **Styling**: Tailwind CSS with custom design tokens and CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Forms**: React Hook Form with Zod validation for type-safe form handling

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM for type-safe database operations
- **Authentication**: JWT-based authentication with bcrypt for password hashing
- **API Design**: RESTful API endpoints with consistent error handling middleware
- **Development**: Hot module replacement with Vite integration for seamless development experience

### Database Design
- **Database**: PostgreSQL with Neon serverless connection
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Tables**: 
  - Users table with authentication and profile data
  - Products table with owner relationships and marketplace fields
  - Cart table for shopping cart functionality
  - Orders and order items tables for purchase history
- **Relationships**: Foreign key constraints ensuring data integrity between users, products, cart items, and orders

### Authentication & Authorization
- **Strategy**: Stateless JWT authentication
- **Password Security**: Bcrypt hashing with salt rounds
- **Session Management**: Token-based authentication stored in localStorage
- **Protected Routes**: Middleware-based route protection with automatic token validation
- **User Management**: Registration, login, and profile management capabilities

## External Dependencies

### Database Services
- **Neon Database**: Serverless PostgreSQL database hosting
- **Connection Pooling**: Built-in connection pooling for optimal database performance

### UI & Styling Libraries
- **Radix UI**: Accessible, unstyled UI primitives for complex components
- **Tailwind CSS**: Utility-first CSS framework for responsive design
- **Lucide React**: Consistent icon library for UI elements
- **Class Variance Authority**: Type-safe variant API for component styling

### Development Tools
- **Vite**: Fast build tool with hot module replacement
- **TypeScript**: Static type checking and enhanced developer experience
- **ESBuild**: Fast JavaScript bundler for production builds
- **Replit Integration**: Development environment optimizations and error overlay

### Form & Validation
- **React Hook Form**: Performant forms with minimal re-renders
- **Zod**: TypeScript-first schema validation
- **Hookform Resolvers**: Integration layer between React Hook Form and Zod

### Utility Libraries
- **Date-fns**: Modern date utility library for date formatting and manipulation
- **Nanoid**: URL-safe, unique string ID generator
- **CLSX/TWMerge**: Conditional className utilities for dynamic styling