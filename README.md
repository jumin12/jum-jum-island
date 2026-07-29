# San Sarabel Island

**Sarabel Island** is a portrait mobile merge-and-serve resort game. Slide pieces, match them, fulfill guest orders, and restore every venue on the island.

Play locally by opening `index.html`, or host the folder as a static site.

The canvas scales to fit mobile, desktop browser windows, and fullscreen (`F` key). Item art lives at `art/merge-pieces.png`.

## Host on Render

This project is a static site (HTML, art, and sounds). No Node build step is required.

1. Push this repo to GitHub (already set up as `san-sarabel-island`).
2. Open the [Render Dashboard](https://dashboard.render.com/).
3. Click **New → Static Site**.
4. Connect the `san-sarabel-island` GitHub repository.
5. Use these settings:
   - **Name:** `san-sarabel-island` (or any name you like)
   - **Branch:** `main`
   - **Build Command:** leave empty, or use `true`
   - **Publish Directory:** `.`
6. Click **Create Static Site**.

Render will give you a free `*.onrender.com` URL and redeploy automatically on every push to `main`.

If you prefer Blueprint deploy, this repo includes `render.yaml`. In the dashboard choose **New → Blueprint** and select the repo.

### Optional custom domain

In the Render service settings, open **Custom Domains**, add your domain, and follow the DNS instructions Render shows.

## Local play

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

Then visit the printed local URL.
