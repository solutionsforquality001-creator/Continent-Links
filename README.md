# Continent Links Storefront

This is a Next.js application. Its homepage is implemented in `src/app/page.tsx`; you do not need to create a separate `index.html` for Vercel.

## Run locally
1. Install Node.js (LTS).
2. Run `npm install`.
3. Copy `.env.example` to `.env.local` and fill in your values.
4. Run `npm run dev` and open the local address shown in the terminal.

## Deploy with GitHub and Vercel
1. Create a new GitHub repository.
2. Upload/extract the contents of this ZIP into the repository root (the `package.json` must be at the root, not inside an extra nested folder).
3. Commit and push the files.
4. In Vercel, import the GitHub repository. Vercel should detect Next.js automatically.
5. In Vercel Project Settings > Environment Variables, set `DATABASE_URL` to your PostgreSQL connection string and `ADMIN_PASSWORD` to a strong password.
6. Deploy.

## Important
The app uses PostgreSQL for database-backed features. Configure a reachable PostgreSQL database before expecting database-backed orders/admin features to work. Never commit `.env.local`, database credentials, or real passwords to GitHub.
