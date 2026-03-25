# YouMove rental valuation page (Vercel)

## Files
- `index.html` - frontend valuation page
- `api/valuation-rent.js` - Vercel serverless function that calls PropertyData securely
- `vercel.json` - Vercel config

## Environment variables
Add this in Vercel:
- `PROPERTYDATA_API_KEY` = your PropertyData API key

## Before you deploy
1. Replace `REPLACE_WITH_GOOGLE_MAPS_BROWSER_KEY` in `index.html` with your browser-restricted Google Maps key.
2. Make sure your Formspree endpoint is correct.
3. Optionally update your Google Ads conversion event.

## Deploy on Vercel
1. Create a new GitHub repo and upload these files.
2. In Vercel, click **Add New > Project**.
3. Import the GitHub repo.
4. In **Environment Variables**, add `PROPERTYDATA_API_KEY`.
5. Deploy.
6. After deploy, test the form with a real UK address.

## Local testing
If you use the Vercel CLI:
1. Install the CLI.
2. Run `vercel dev` inside the project folder.
3. Add the env var when prompted or via `.env.local`.
