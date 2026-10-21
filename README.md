# Meadow House — Discord Community Website

Cute meadow-themed responsive React + Vite starter.

## Features in this demo
- Responsive mobile navigation
- Home dashboard, sample stats, community feed, likes, search, and post composer
- Personal garden, once-per-browser-session daily watering reward, coins, inventory, and item shop
- Event list and local RSVP toggles
- Suggestions form UI
- Bot feature planning page
- English/Thai UI switch
- Demo state stored in browser localStorage

## Important limitations
This is a front-end demo, not a production platform:
- No Discord login, server membership checks, live Discord data, or bot API connection.
- Posts, likes, coins, garden progress, inventory, and event RSVP state stay only in the current browser on this device.
- The suggestion form does not send or save submissions.
- Statistics, members, and events are placeholders.
- Do not collect sensitive information with this demo.
- Before launch, add a secure backend/database, moderation/reporting, server-side validation, privacy disclosures, and appropriate access rules. Never put a Discord bot token, OAuth client secret, or database service-role key in frontend code.

## Deploy from iPhone with GitHub + Vercel
1. Download and unzip this project.
2. In GitHub, create a repository such as `meadow-house`.
3. Upload the contents of the project, keeping `src` as a folder:
   - `package.json`
   - `index.html`
   - `src/main.jsx`
   - `src/App.jsx`
   - `src/styles.css`
   - `README.md`
4. In Vercel, choose **Add New → Project**, then import the GitHub repository.
5. Use these settings if Vercel doesn't detect them automatically:
   - Framework preset: **Vite**
   - Build command: `npm run build`
   - Output directory: `dist`
   - Install command: `npm install`
6. Tap **Deploy**. New commits to the connected branch redeploy automatically.

If the GitHub iPhone app doesn't show file-creation/upload options, open GitHub in Safari and use the repository website. Uploading files is easier than pasting a huge file into the editor.

## Change Discord invite
In `src/App.jsx`, edit:
```js
const INVITE = 'https://discord.gg/dbExmqRypP';
```

## Change fonts
`index.html` imports Mali and DM Sans from Google Fonts. Main headings use Mali; most body text uses DM Sans. Change the Google Fonts import and CSS font-family values in `src/styles.css` if you want another style.
