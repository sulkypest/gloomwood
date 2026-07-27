# Gloomwood — Ross Young Author Site

Single-page author site for Ross Young, author of the Gloomwood novels
(*Dead Heads*, *Get Ted Dead*, *Dead Festive*, *Dead Culture*).

Everything lives in `index.html` — no build step, no dependencies. Book covers
and the author photo are hotlinked from Goodreads/Amazon and bio.link, so an
internet connection is needed to see them (fine for a live site).

## Publish it with GitHub Pages

1. Create a new repo on GitHub named `gloomwood` (public).
2. From this folder, run:

   ```
   git remote add origin https://github.com/<your-username>/gloomwood.git
   git branch -M main
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`. Save.
4. After a minute or two your site is live at:
   `https://<your-username>.github.io/gloomwood/`

## Pointing your existing domain at it

Once the Pages URL works, you can either:
- Add a link from your current site (rossyoung.ink) to the new Pages URL, or
- Point rossyoung.ink's DNS at GitHub Pages directly (add a `CNAME` file with
  `rossyoung.ink` in it, and set an `A`/`ALIAS` record at your DNS provider to
  GitHub Pages' IPs — see GitHub's "Managing a custom domain" docs).

## Future updates

Edit `index.html` directly, commit, and push — Pages redeploys automatically
within a minute or so.
