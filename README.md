# Evently Frontend

React and Vite frontend for the Web Based Event Enrollment System.

## Run locally

Install Node.js, start the Spring Boot backend on `http://localhost:8080`, then run:

```powershell
npm install
npm run dev
```

Open `http://localhost:5173`. The frontend sends API requests to `http://localhost:8080/api` and uses the backend session cookie.

## Deploy the frontend

For a Vercel deployment, import this repository, keep the project root at the repository root, use `npm run build` as the build command, and `dist` as the output directory. Add `VITE_API_BASE_URL` in the Vercel project settings with the deployed backend API URL, ending in `/api` (for example, `https://your-api.onrender.com/api`). Deploy again after setting the variable. The rewrite configuration supports React Router URLs such as `/events` on refresh.
