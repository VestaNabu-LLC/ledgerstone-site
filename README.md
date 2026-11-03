# Ledgerstone website

Public site for Ledgerstone by Monaidea, served by GitHub Pages at https://ledgerstone.monaidea.com.

Contact form (owner request, 2026-11-02): `/support/` has the same form as https://www.monaidea.com, and the site's other calls to action link to it (`/support/#contact`, with `?topic=early-access` and similar to preselect a topic). `contact.js` is a copy of the file in VestaNabu-LLC/monaidea; keep the three copies (monaidea, ledgerstone-site, flagstone-site) identical and bump `?v=` on its script tag when it changes. The form posts to Monaidea's contact Worker at https://forms.monaidea.com (source and tests in the monaidea repo's `worker/`), which checks Cloudflare Turnstile and emails support@monaidea.com through Postmark; `data-product` on the form puts the app's name in the email's subject.
