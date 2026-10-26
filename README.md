# Glingos Battle

A small browser multiplayer prototype using the original `en.png` and `um.png` sprites.

## Publish on GitHub Pages
1. Create a GitHub repository named `glingos-battle`.
2. Upload `index.html`, `en.png`, and `um.png` to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/(root)`, then Save.
5. Wait for the published URL to appear on the Pages settings screen.

## Configure multiplayer
1. Create a project in https://supabase.com/dashboard.
2. Copy the project URL and the publishable key (or legacy anon key) from the project's API settings.
3. Open the published site, paste both into the connection fields, and choose a room code.
4. Click **Connect / Join room**. Give your friend the website URL, the same project URL, the same publishable/anon key, and the same room code.

Do not use or share a Supabase service-role/secret key in this page or repository.

## Prototype limitations
This is a starter prototype, not a cheat-resistant production multiplayer game. It uses browser Broadcast messages, so game state and scoring are not server-authoritative. For a robust competitive version, move collision detection, scoring, room membership, and validation to a trusted backend. This version is intended to get the sprites, connection flow, and basic movement prototype running first.
