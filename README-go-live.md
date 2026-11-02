# Barndo Beam Co. site (ready, NOT live yet)

Planned link: https://malinda-commits.github.io/barndo-beam-co/
Planned repo: https://github.com/malinda-commits/barndo-beam-co (public, branch `main`, folder `/`)

## To go live (about 3 minutes, free)
Cursor's GitHub connection can't create repos, so this step is yours:
1. On github.com, click New repository, name it `barndo-beam-co`, choose Public, then Create.
2. Click "uploading an existing file" and drag in everything from `barndo-beam-co-site.zip` once it's unzipped (index.html, products.js, favicon.png, .nojekyll, img/). Then Commit.
3. Go to Settings, then Pages, choose Deploy from a branch, pick `main` and `/ (root)`, then Save. It's live in about a minute.

It's a plain static site (index.html, products.js, img/, favicon.png, .nojekyll) with no build step and no server.

## Products
`products.js` is generated. Don't edit it by hand. Edit `/workspace/stores/beams/products_data.py`, then run `python3 make_listings.py`. That one command keeps the site, listings.csv, listings.md and pricing.md in sync. Then push products.js to the repo.

## Quote form
The form opens the shopper's email app addressed to **malinda@scottbuilt.com** with the subject **"Barndo Beam Co. quote request"**. The item, ZIP and details are filled into the body. Change `QUOTE_EMAIL` / `QUOTE_SUBJECT` in index.html if needed.
To use a free Google Form instead, paste its link into `GOOGLE_FORM_URL`.

## Later (optional)
- Keep her name out of the link with a free GitHub organization `barndobeamco`, which gives https://barndobeamco.github.io/
- Point a domain like barndobeamco.com (about $10 to $15/yr, needs her OK) at the same site.
- Swap the AI concept photos for real photos of the pieces.
