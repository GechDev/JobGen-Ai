# JobGen

A comprehensive job search and application platform built with Next.js frontend and Go backend.

## Features

- Job search and filtering
- Resume upload and parsing with AI
- User authentication and profiles
- Chat functionality for job inquiries
- Contact forms and support

## Tech Stack

- **Frontend**: Next.js, TypeScript, Tailwind CSS
- **Backend**: Go, Gin framework, MongoDB
- **AI Integration**: OpenAI API for resume analysis
- **Authentication**: NextAuth.js

## Getting Started

### Prerequisites

- Node.js 18+
- Go 1.19+
- MongoDB
- Docker (optional)

### Installation

1. Clone the repository
2. Install frontend dependencies: `cd frontend && npm install`
3. Install backend dependencies: `cd jobgen-backend && go mod download`
4. Set up environment variables
5. Run the application: `npm run dev` for frontend, `go run main.go` for backend

## Contributing

Please read CONTRIBUTING.md for details on our code of conduct and the process for submitting pull requests.

## API Documentation

The API documentation is available via Swagger at `/swagger/index.html` when the backend is running.

## Environment Variables

Create a `.env` file in the backend directory with the following variables:

- `MONGO_URI`: MongoDB connection string
- `JWT_SECRET`: JWT signing secret
- `OPENAI_API_KEY`: OpenAI API key for AI features
- `EMAIL_USER`: Email service username
- `EMAIL_PASS`: Email service password

## Deployment

The application can be deployed using Docker:

```bash
docker-compose up -d
```