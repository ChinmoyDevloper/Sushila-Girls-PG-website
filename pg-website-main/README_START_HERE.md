# Sushila Girls PG Website

Yellow / black / white theme, girls-PG wording, no photos needed.

## Run locally
1. Extract the ZIP and open the `pg-website-main` folder in VS Code.
2. Right-click `index.html` -> Open with Live Server.
3. Admin page: `/admin/index.html` on the same address.

## Logo
The yellow bed icon is `images/logo.png` (navbar, footer, browser tab). The full logo with text is `images/logo-full.png`.

## Hero photo
The homepage background is `images/hero.jpg` (a wide, landscape photo works best). Room card photos are `images/room-1.jpg`, `room-2.jpg`, `room-3.jpg`.

## Things you must set before going live
- `script.js`: set `WHATSAPP_NUMBER` and `MAPS_LINK`.
- Phone and address: edit in the admin panel, or in `index.html`.
- Rent, deposit, rooms and facilities: only publish confirmed details.

## IMPORTANT: Firebase
`firebase-config.js` still points to the ORIGINAL Acharya Boys PG Firebase project.
Create a NEW Firebase project for Sushila Girls PG, paste its config into `firebase-config.js`,
create a new admin user, put that user's UID in `admin/admin.js` and `firestore.rules`,
then publish the rules. Otherwise both PGs share the same enquiries and admin login.
