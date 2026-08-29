# React Projects Selection

### Collection of practical React projects covering component-based UI development, state management, hooks, routing, external APIs, and client-side application patterns

This repository contains a selection of small React applications and exercises created during structured front-end learning and hands-on practice.

The projects progress from fundamental component and state concepts toward more involved examples using React hooks, Context API, reducers, routing, external APIs, browser storage, and Firebase / Firestore.

The repository is retained as supporting evidence of practical React experience. My current engineering focus is primarily .NET and backend development.

---

## Concepts Covered

Across the project collection, the examples include:

- reusable React components and props
- local component state with `useState`
- side effects and asynchronous data loading with `useEffect`
- shared state with Context API and `useContext`
- reducer-based state management with `useReducer`
- DOM references with `useRef`
- memoized callbacks with `useCallback`
- forms and controlled inputs
- conditional rendering
- list rendering and component composition
- React Router navigation and route parameters
- external REST API consumption
- pagination and infinite scrolling
- browser persistence with `localStorage`
- Firebase / Firestore integration

---

## Project Collection

The repository contains 28 focused projects:

```text
01-birthday-reminder
02-tours
03-reviews
04-accordion
05-menu
06-tabs
07-slider
08-lorem-ipsum
09-color-generator
10-grocery-bud
11-navbar
12-sidebar-modal
13-stripe-submenus
14-cart
15-cocktails
16-markdown-preview
17-random-person
18-pagination
19-stock-photos
20-dark-mode
21-movie-db
22-hacker-news
23-quiz
24-react-info-website
25-airbnb-clone
26-meme-generator
27-notes-app
28-tenzies-game
```

The collection includes both focused UI exercises and projects involving application state, routing, persistence, and external services.

---

## Selected Examples

### Cart

Demonstrates shared application state using React Context and `useReducer`, together with asynchronous data loading and cart operations.

### Cocktails

Uses React Router, Context API, hooks, and external API communication to provide search and detail workflows.

### Stock Photos

Demonstrates external API consumption, `useRef`, dynamic loading, and infinite-scrolling behavior.

### Movie DB

Uses React Router, route parameters, external API integration, Context API, and reusable data-fetching logic.

### Hacker News

Combines Context API, `useReducer`, asynchronous API communication, search, and pagination.

### Quiz

Uses Context-based state, Axios, form input, and an external trivia API to provide configurable quiz workflows.

### Notes App

Implements note management with React and Firebase / Firestore persistence. Firebase client configuration is supplied through Vite environment variables rather than being tied to a specific Firebase project in source control.

### Tenzies

A small interactive game centered on component state, derived UI state, and user interaction.

---

## External API Configuration

Some projects require API credentials or external service configuration.

### Stock Photos

Create a local environment file in `19-stock-photos` and provide:

```dotenv
REACT_APP_ACCESS_KEY=your-unsplash-access-key
```

### Movie DB

Create a local environment file in `21-movie-db` and provide:

```dotenv
REACT_APP_MOVIE_API_KEY=your-omdb-api-key
```

### Notes App

Copy:

```text
27-notes-app/.env.example
```

to:

```text
27-notes-app/.env.local
```

and provide the Firebase client configuration for your own Firebase project.

Local environment files are excluded from source control.

---

## Running a Project

Each folder is an independent React application with its own dependencies.

Navigate to the project you want to run, for example:

```bash
cd 15-cocktails
npm install
npm start
```

Projects using Vite, such as `27-notes-app`, can instead be started with:

```bash
cd 27-notes-app
npm install
npm run dev
```

Because these projects were created across different stages of React study, dependency versions and tooling vary between projects.

---

## Technology

JavaScript · React · React Hooks · Context API · React Router · REST APIs · Axios · Firebase / Firestore · localStorage · Create React App · Vite

---

## Repository Scope

This repository is intentionally a collection of learning-oriented React projects rather than a single production application.

The projects were created to practice React concepts in isolation and in progressively more complete application scenarios. Some use older React versions or tooling that reflects the period in which the exercises were completed; they are retained as examples of hands-on front-end experience rather than actively maintained production applications.