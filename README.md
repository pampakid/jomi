# Jomi - Real Estate App for Argentine Market

Jomi is a comprehensive real estate platform designed specifically for the Argentine market, consisting of three main components:

- Backend API (Python/FastAPI)
- Mobile App (React Native)
- Admin Dashboard (React)

## Project Structure

```
jomi/
├── backend/           # FastAPI backend
├── mobile-app/       # React Native mobile app
└── admin-dashboard/  # React admin dashboard
```

## Prerequisites

- Python 3.11+
- Node.js 18+
- PostgreSQL 14+
- React Native development environment

## Getting Started

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

5. Run the development server:
   ```bash
   uvicorn app.main:app --reload
   ```

### Mobile App Setup

1. Navigate to the mobile app directory:
   ```bash
   cd mobile-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Run on iOS/Android:
   ```bash
   npm run ios
   # or
   npm run android
   ```

### Admin Dashboard Setup

1. Navigate to the admin dashboard directory:
   ```bash
   cd admin-dashboard
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

## Development

- Follow the [Contributing Guidelines](CONTRIBUTING.md)
- Use the provided pull request template
- Ensure all tests pass before submitting PRs

## Testing

### Backend Tests
```bash
cd backend
pytest
```

### Mobile App Tests
```bash
cd mobile-app
npm test
```

### Admin Dashboard Tests
```bash
cd admin-dashboard
npm test
```

## Deployment

The project uses GitHub Actions for CI/CD. Each component has its own deployment configuration:

- Backend: Deploys to [your backend hosting service]
- Mobile App: Deploys to App Store and Google Play Store
- Admin Dashboard: Deploys to [your frontend hosting service]

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 