# Delta Script Hub

Initial website for Delta Script Hub.

## Deploy to Cloudflare Pages
1. Connect this GitHub repository to Cloudflare Pages.
2. Select `main` as the production branch. For this plain HTML site, leave the build command blank and set the output directory to `/`.
3. Deploy.

## Admin/database setup
The current `index.html` is the initial public landing page and search UI. It does **not yet implement a real admin login or script publishing workflow**.
To add that securely, create a Supabase project, run `supabase-schema.sql` in its SQL Editor, create an admin account in Supabase Auth, and add its user ID to `public.admins`. Do not expose a Supabase service-role key in browser code. The front-end must then be connected to Supabase Auth and the scripts table.

Footer brand: `CLOUDFLARE • © 2026`.
