# Agrositrus — Premium Liquid-Glass Site (Starter)

**What you get**
- Vite + React frontend with "liquid glass" aesthetic.
- Supabase-ready integration for Auth, Posts, Products, and Storage.
- Admin panel (email login via Supabase) and fallback localStorage demo mode.
- Seed SQL for Supabase (tables + sample rows).
- Tailwind CSS setup.

**Quick start (local)**
1. Install dependencies:
   ```bash
   npm install
   ```
2. Copy `.env.example` to `.env` and fill your Supabase keys (optional).
   - If you do not configure Supabase, the app will run in **demo/local** mode using `localStorage`.
3. Start development server:
   ```bash
   npm run dev
   ```
4. Open `http://localhost:5173` (or the URL shown by Vite).

**Supabase setup (recommended for full features)**
1. Create a project at https://app.supabase.com
2. In the SQL editor run `supabase/schema.sql` to create tables and seed data.
3. Create a Service Role or use anon public key for client-side (anon is recommended for client).
4. Set `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY` in `.env` (see `.env.example`).
5. Deploy to Vercel (recommended) — set the same env vars in Vercel dashboard.

**Files of interest**
- `src/` — React source
- `supabase/schema.sql` — DB schema + seed data
- `README.md` — this file

**Security note**
- This starter uses Supabase client directly from frontend. Configure RLS (Row Level Security) in Supabase to secure writes.
- Replace demo admin password and enable proper auth flows before production.

If you want, I can also:
- Provide a ready GitHub repo,
- Configure Vercel deployment instructions,
- Add payment/integration (Stripe/Payme) examples,
- Or convert admin to server-side secure functions.

Enjoy — Agrositrus team! 🌱🍊
