# My Watchlist App 🎬📚

This project is a full-stack web application where users can search for media (movies, TV shows, etc.) and manage their personal watchlist. This project is being built collaboratively by a Frontend Lead/Mentor and a Backend Apprentice.

## Tech Stack

- **Frontend:** [React](https://reactjs.org/), [TailwindCSS](https://tailwindcss.com/), [TypeScript](https://www.typescriptlang.org/)
- **Backend:** [NestJS](https://nestjs.com/), [PostgreSQL](https://www.postgresql.org/)
- **ORM:** [TypeORM](https://typeorm.io/)
- **Deployment:** [Docker](https://www.docker.com/)

## Project Structure

This project is a monorepo with the following structure:

- `/client`: Contains the React.js frontend application.
- `/api`: Contains the NestJS backend application.

## Project Plan

This project is divided into the following phases:

### Phase 1: Foundation & Setup
- [x] **Project Scaffolding:** Set up a monorepo with `/client` and `/api` directories. Initialize Git.
- [ ] **Dockerization:** Create `docker-compose.yml` and `Dockerfile`s for client, api, and db.
- [x] **Initialize Apps:** Use CLIs to create boilerplate for React and NestJS.
- [ ] **Database Integration:** Integrate TypeORM into the NestJS project and define initial schema.

### Phase 2: Public Media Search
- [ ] **API - Health Check:** Create a `GET /health` endpoint.
- [ ] **API - Search Endpoint:** Create a `GET /media/search` endpoint.
- [ ] **Frontend - UI Components:** Build `SearchBar`, `MediaCard`, and `SearchResultsGrid` components.
- [ ] **Frontend - Integration:** Connect the UI to the search API endpoint.

### Phase 3: User Authentication
- [ ] **API - Signup:** Implement `POST /auth/signup` endpoint.
- [ ] **API - Login:** Implement `POST /auth/login` endpoint with JWT.
- [ ] **Frontend - Auth Pages:** Build UI for `/signup` and `/login`.
- [ ] **Frontend - State Management:** Set up global state for authentication.
- [ ] **Frontend - Integration:** Connect auth forms to the API.

### Phase 4: Personal Watchlists
- [ ] **API - Route Protection:** Implement a Guard for protected routes.
- [ ] **API - CRUD Operations:** Implement `POST`, `GET`, `DELETE` for `/watchlist`.
- [ ] **Frontend - Add/Remove UI:** Add "Add to Watchlist" button.
- [ ] **Frontend - Watchlist Page:** Create the `/watchlist` page to display and manage items.

### Phase 5: Refinement & Error Handling
- [ ] **API - Validation & Error Handling:** Implement validation pipes and DTOs.
- [ ] **Frontend - UI States:** Implement loading and empty states.
- [ ] **Frontend - Error Handling:** Display user-friendly error messages.
- [ ] **Frontend - Protected Routes:** Redirect unauthenticated users.

### Phase 6: Deployment & Next Steps
- [ ] **Production Prep:** Use environment variables for secrets.
- [ ] **Deployment:** Deploy client, api, and database.
- [ ] **Celebrate & Plan:** Brainstorm future features.

## Getting Started

To get the development environment running, you will need to have [Docker](httpss://www.docker.com/get-started) installed.

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd watch-list
    ```

2.  **Run the application:**
    ```bash
    docker-compose up --build
    ```

This will start three services:
- `client`: The React frontend, accessible at `http://localhost:3000`
- `api`: The NestJS backend, accessible at `http://localhost:3001`
- `db`: The PostgreSQL database.

## Roles

- **Frontend Lead & Mentor:** Zehao Xue
- **Backend Apprentice:** Michael Cabanas
