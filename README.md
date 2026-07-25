# Personal site — Pratik Palkar

Static single-page site for GitHub Pages. No build step, no dependencies.

**Live URL:** https://pratikpalkar1703-gif.github.io/seo-geo-project-manager/

## Files to upload

| File | Purpose |
|---|---|
| `index.html` | The whole site — HTML, CSS and JSON-LD in one file |
| `Pratik_Palkar_Resume.pdf` | CV, linked from the nav and both download buttons |
| `llms.txt` | Plain-text summary for AI crawlers |

`README.md` is optional — it shows on the repo page, not the site.

## Publishing

1. Create the repo: **`seo-geo-project-manager`**, owner `pratikpalkar1703-gif`, visibility **Public**.
2. On the empty repo page click **uploading an existing file** and drag in `index.html`, `Pratik_Palkar_Resume.pdf` and `llms.txt`. Commit.
3. **Settings → Pages** → Source: **Deploy from a branch** → Branch `main`, folder `/ (root)` → **Save**.
4. Wait 1–2 minutes, then open the live URL above. First deploy occasionally takes 5.

All URLs in `index.html` are already set to this address — nothing to edit before uploading.

## After it's live

- Run the URL through [validator.schema.org](https://validator.schema.org/) to confirm the entity graph parses.
- Add the property in **Google Search Console** and request indexing.
- Put the link on your LinkedIn profile and in the contact line of your CV.

## If you buy a domain later

1. Add a file named `CNAME` (no extension) to the repo root containing just `pratikpalkar.com`.
2. At your registrar, create four A records for the apex pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`, and a CNAME for `www` pointing to `pratikpalkar1703-gif.github.io`.
3. **Settings → Pages → Custom domain**, enter the domain, tick **Enforce HTTPS**.
4. Find-and-replace every instance of `https://pratikpalkar1703-gif.github.io/seo-geo-project-manager/` in `index.html` and `llms.txt` with `https://pratikpalkar.com/`.

Step 4 matters — the canonical tag and the JSON-LD `@id` values must match the live URL, or you end up with two competing versions of the same entity.
