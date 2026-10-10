# Zoë Austin Portfolio

Portfolio site for Zoë Austin, multimedia creative.

| What | Where |
| --- | --- |
| Home page | `index.html`, with images in `assets/` |
| Case study | `password-protected/` (Password Protected, Victoria's Secret spec campaign) |
| Netlify site | https://zoeportfoliosite.netlify.app |
| Loader block | `loader/zoe-austin.html` |

Static files only, no build step. `netlify.toml` publishes the repo root.

## Set up the loader (one time)

1. Open the page in the site builder and add a **Code** widget (Readymag) or **Code** block (Squarespace).
2. Paste the contents of `loader/zoe-austin.html`. In Readymag, leave **Use iFrame** off.
3. Check it in **Preview**, since editors may not run custom code.
4. Publish.

On each visit the loader asks GitHub for the newest commit on `main` and loads that exact version through jsDelivr, so a push shows up on the next visit. Links between the home page and the case study stay inside the frame. If jsDelivr fails it falls back to the Netlify site.
