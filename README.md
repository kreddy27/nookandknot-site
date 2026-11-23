# Nook And Knot website

A static, one-page website for the custom gift collection. No build step, no dependencies, no tracking.

## Files

- `index.html` : the home page (hero, collection, occasions, how it works, about, contact)
- `privacy.html` : privacy policy
- `terms.html` : terms of sale
- `style.css` : all styling

## Preview locally

From this folder:

    python -m http.server 8090

Then open http://127.0.0.1:8090/

## Before you publish: check these

1. **Contact details** on `index.html`, `privacy.html` and `terms.html`: the address and the phone number are copied from the Meta business portfolio. Change them if they are wrong or if you do not want the phone number public.
2. **An email address**: there is none on the site. Meta verification and customers may expect one, so add a business email (ideally on nookandknot.shop) to the Contact section and to both legal pages.
3. **The legal pages are plain, generic drafts**, not legal advice. Have them reviewed, especially delivery times, cancellations, returns and the governing-law clause, and edit them to match how you actually run orders.
4. **Collection and wording**: the four collection cards and the occasion list are generic. Replace them with what you actually make. There are no product photos yet; real photos would improve it a lot.
5. **If you add analytics, a contact form or a payment button later**, update the privacy policy, which currently says the site uses no cookies or tracking.

## Publish (free hosts)

Any of these work: upload the whole folder.

- **Cloudflare Pages** (recommended): Workers & Pages > Create > Pages > Upload assets, upload this folder, then add the custom domain `nookandknot.shop`.
- **Netlify**: app.netlify.com > Add new site > Deploy manually, drag the folder in, then add the custom domain.
- **GitHub Pages**: put these files in a repository, enable Pages, then add the custom domain.
- **Vercel**: import this repository at vercel.com/new. It is a plain static site, so keep the Framework Preset as "Other" and leave the build command and output directory empty (the root folder is served). Then add the domain under Project > Settings > Domains and add the DNS records Vercel shows at your registrar. Note: Vercel's free Hobby plan is for non-commercial use under its terms; a business site may need a paid plan, so check Vercel's current terms before relying on it.

Then point the domain's DNS at the host (the host shows the exact record to add at your registrar), wait for it to load over https, and set the website field on the Meta business portfolio to `https://nookandknot.shop`.
