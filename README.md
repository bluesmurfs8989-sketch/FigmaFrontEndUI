
  # Campus Events Hub UI Design

  This is a code bundle for Campus Events Hub UI Design. The original project is available at https://www.figma.com/design/0ZpvDaaPTcVSladgJF6cuD/Campus-Events-Hub-UI-Design.

  ## Running the code

  Run `npm i` to install the dependencies.

  Run `npm run dev` to start the development server.

  ## Backend (free, demo API)

  A lightweight Express API is included for local use (no hosted costs):
  - `cd backend && npm install`
  - `npm start` (runs on http://localhost:4000)
  - Frontend will use `VITE_API_BASE_URL` if set; otherwise defaults to http://localhost:4000 with a fallback to local sample data when the API is down.
  - Registrations and updated counts are now persisted to `backend/data/registrations.json` and `backend/data/events.json` (JSON on disk) while the server is running.
  - Create events via `POST /api/events` (fields: name, shortDescription, fullDescription, date, time, location, category, capacity, hostedBy, optional imageUrl).
  
