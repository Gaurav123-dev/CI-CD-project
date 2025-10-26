# CI/CD example

This repo demonstrates:
- CI: tests & lint via GitHub Actions
- CD: build Docker image and publish to GitHub Container Registry
- Static frontend deployment to GitHub Pages

core CI/CD (GitHub Actions + GitHub Pages + GHCR).

## How to run locally
### Backend
cd backend
npm ci
npm test
npm start
## Docker
docker build -t ci-cd-backend:local ./backend
docker run -p 3000:3000 ci-cd-backend:local
