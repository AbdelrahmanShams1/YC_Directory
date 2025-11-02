# Next.js Application with Advanced Architecture

## Project Overview

A modern Next.js web application built with a sophisticated architecture that includes AWS integration, authentication capabilities, and development tooling. The project demonstrates enterprise-grade patterns with proper dependency management and development workflows.

## Tech Stack

### Core Technologies
- **Next.js** - React framework for production
- **Node.js** - Runtime environment
- **TypeScript** - Type safety and developer experience

### Key Dependencies
- **@auth/core** (v0.41.0) - Authentication system
- **@architect** suite - Serverless application toolkit
  - `@architect/hydrate` - Dependency management
  - `@architect/inventory` - Resource enumeration
  - `@architect/asap` - Static asset proxy
  - `@architect/parser` - Manifest parsing
  - `@architect/utils` - Common utilities
- **@aws-lite** - Lightweight AWS client with plugins for:
  - S3, SSM, DynamoDB, Lambda, and other AWS services
- **Babel** - JavaScript compiler and transpiler
- **Preact** - Lightweight React alternative

### Development Tools
- **ESLint** - Code linting
- **Tape** - Testing framework
- **NYC** - Code coverage
- **Vite** - Build tool for some components
- **VS Code** with MCP (Model Context Protocol) configuration

## Architecture

### Serverless-First Approach
The project is designed with serverless architecture in mind, leveraging AWS Lambda and related services through the Architect framework.

### Modular Design
- **Plugin-based AWS integration** using `@aws-lite` plugins
- **Dependency hydration system** for optimal package management
- **Static asset optimization** with ASAP (Architect Static Asset Proxy)

### Authentication Ready
Integrated with Auth.js for comprehensive authentication supporting:
- OAuth/OpenID Connect
- JWT tokens
- WebAuthn for passwordless authentication
- Email authentication with nodemailer

## Features

- ✅ **Next.js App Router** - Modern React server components
- ✅ **AWS Integration** - Full suite of AWS services
- ✅ **Authentication System** - Multi-provider auth support
- ✅ **Static Asset Delivery** - Optimized asset serving
- ✅ **Development Tooling** - Comprehensive testing and linting
- ✅ **TypeScript Support** - Full type safety
- ✅ **Serverless Deployment Ready** - Architect framework integration

## Testing

The project includes a robust testing setup:


# Run tests
npm test

# Test with coverage
npm run coverage

# Integration tests
npm run test:integration

# Live testing
npm run test:live  


How to Run the Project
Prerequisites
Node.js >= 16

npm or yarn

Installation
bash
# Install dependencies
npm install

# Development mode
npm run dev

# Production build
npm run build

# Start production server
npm start
Environment Setup
Clone the repository

Install dependencies: npm install

Set up environment variables (if required)

Run development server: npm run dev

Open http://localhost:3000

Development Scripts
bash
npm run dev      # Start development server
npm run build    # Create production build
npm run test     # Run test suite
npm run lint     # Run linter
npm run coverage # Generate test coverage report
