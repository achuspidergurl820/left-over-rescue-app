# Leftover Rescue

A simple, Vercel-ready prototype for a hyper-local surplus food marketplace.

## Run on your computer

No Python or database is required for this version.

1. Open the project folder.
2. Double-click `index.html` to test it, or use VS Code Live Server.
3. Try **Find food nearby**.
4. Try **List surplus food**.
5. Add a listing and refresh the page. It is stored in your browser using `localStorage`.

## Deploy to Vercel

### Option A — GitHub + Vercel

1. Create a new GitHub repository, for example `leftover-rescue`.
2. Upload `index.html` and this `README.md`.
3. Open Vercel and choose **Add New Project**.
4. Import the GitHub repository.
5. For this static project:
   - Framework preset: **Other**
   - Build command: leave empty
   - Output directory: leave empty
6. Deploy.

Vercel will serve `index.html` as the homepage.

### Option B — Vercel CLI

Install Node.js first, then in this folder run:

```bash
npx vercel
```

Follow the prompts. For production:

```bash
npx vercel --prod
```

## Important next step for a real marketplace

This prototype stores listings only in each visitor's browser. For a real multi-user app, connect a backend such as Supabase or Firebase for:

- accounts and login
- real listings shared between users
- pickup reservations
- location/area search
- seller verification
- image uploads
- notifications
- reporting/moderation
- admin dashboard

The current UI can be kept while replacing the `localStorage` layer with a database API.
