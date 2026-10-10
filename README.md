# SocietyConnect — Static Preview Hosting Package

This package hosts the existing SocietyConnect HTML prototype as a static preview. The `index.html` file is copied unchanged from `SocietyConnect_Banking_UI_V101.html`.

## Deploy to Vercel using GitHub
1. Create a new GitHub repository named `societyconnect-preview` (public or private, as you prefer).
2. Upload `index.html`, `vercel.json`, and this README to the repository root.
3. In Vercel, choose **Add New → Project**, import the GitHub repository, and deploy.
4. Use the generated `*.vercel.app` URL to test the prototype.

## Important limitations
- This is only a static UI preview. The HTML currently contains no Supabase client initialization (`createClient`) and does not connect to the database.
- Hosting does not make authentication, role permissions, financial transactions, or persistence functional.
- Do not enter real member, financial, or sensitive information in this preview.
- Do not put a Supabase `service_role` key in frontend code. When later connecting Supabase, use only the project URL and public anon/publishable key in the browser, with correctly tested RLS policies.
- The database security SQL files are not included in the website root and are not automatically executed by deployment.
