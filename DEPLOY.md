# Deploy Checklist — infinite4you.com

Your fixed site is **`index.html`** (founder photo embedded, no leaking CSS, working
countdown/enroll, mobile-responsive). It lives in this branch. To go live:

## Your live site repo
`aiguru110-svg/turbo-octo-adventure`  (GitHub Pages → infinite4you.com)

> Note: I could NOT edit that repo from this session — it's under a different
> GitHub owner (aiguru110-svg) than this session's repo (joeyvssandc-collab),
> and cross-owner edits are blocked. So upload it yourself with the steps below,
> OR start a NEW Claude session with `aiguru110-svg/turbo-octo-adventure` as the
> repo and I'll edit it directly + open a pull request.

## Option A — Upload it yourself (~5 min, live today)
1. Go to **github.com/aiguru110-svg/turbo-octo-adventure**
2. **Add file ▾ → Upload files** → drag in `index.html` (and `founder-avatar.jpg`)
   → **Commit changes** to the default branch (`main`/`master`). This replaces the old index.html.
3. **Add file ▾ → Create new file** → name it exactly `CNAME` → content:
   ```
   infinite4you.com
   ```
   → **Commit changes**.  (Deleting the old CNAME is what disconnected your domain — this fixes it.)
4. **Settings → Pages** → Source = *Deploy from a branch*, branch = default, folder = **/ (root)**.
   Custom domain should read `infinite4you.com`.
5. Wait 1–3 min → open **infinite4you.com**.

## After it's live — still TODO
- The email only had the HERO section, so Curriculum / Wins / Pricing / FAQ are
  **placeholders**. Paste me the real content and I'll drop it in.
- In `index.html`, set:
  - `CHECKOUT_URL` (near bottom, in the script) → your Stripe/checkout link for the Enroll buttons.
  - `DEADLINE` → your real cohort close date (currently 7 days from page load).

## Also in progress (Etsy side)
- Ultimate Finance Bundle: 4 printable PDFs (Budget, Savings, Debt Payoff, Meal) + combined 26-page PDF.
- 12 watermarked "SAMPLE" listing images (cover + 2 sample pages per product).
- Next options discussed: bundle hero image, editable Canva version, recolor variations,
  and a "Free Printables"/shop section on the site linking to Etsy.
