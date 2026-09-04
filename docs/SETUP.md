# Setup Guide

## Prerequisites

- .NET 8+ SDK
- Node.js 18+
- SQL Server (local or cloud)
- Git

## Backend Setup

1. Navigate to src folder:
   ```bash
   cd src
   ```

2. Install dependencies:
   ```bash
   dotnet restore
   ```

3. Configure database connection in `appsettings.json`

4. Run migrations:
   ```bash
   dotnet ef database update
   ```

5. Start the API:
   ```bash
   dotnet run --project WebAPI
   ```

Server runs on: `http://localhost:5000`

## Frontend Setup

1. Navigate to ClientApp folder:
   ```bash
   cd ClientApp
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Update API endpoint in environment files if needed

4. Start development server:
   ```bash
   npm start
   ```

Application runs on: `http://localhost:4200`

## Environment Variables

1. Copy `.env.example` to `.env`
2. Update values with your configuration
3. Never commit `.env` file

## Verification

- Backend: Visit `http://localhost:5000/api` endpoints
- Frontend: Visit `http://localhost:4200`
- Check browser console for errors
