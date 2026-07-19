Tina Done It Website
====================

Email used on website: hello@tinadoneit.com.au

Site structure
--------------
- index.html            Homepage
- free-resources.html    Free AI Resources page
- assets/logo-icon.png   Nav logo
- assets/favicon.ico, favicon-16x16.png, favicon-32x32.png,
  apple-touch-icon.png, android-chrome-192x192.png,
  android-chrome-512x512.png, site.webmanifest
                         Favicon set (kept from the previous build)

How to deploy on Cloudflare Pages
---------------------------------
This repo is deployed straight from GitHub, so there is no ZIP to extract
or manually upload.
1. In Cloudflare, go to Workers & Pages > Create > Pages > Connect to Git.
2. Select this GitHub repository (tinadoneit/tinadoneit-portfolio).
3. Use these settings:
   - Framework preset: None
   - Build command: leave blank
   - Build output directory: /
4. Deploy.
5. Go to Custom Domains and add:
   - tinadoneit.com.au
   - www.tinadoneit.com.au
Every push to main redeploys automatically once this is set up.

Google Analytics setup
-----------------------
Neither page currently ships a GA4 snippet. To add one:
1. Create a GA4 property at analytics.google.com.
2. Copy your Measurement ID. It looks like G-XXXXXXXXXX.
3. Paste this into <head> of both index.html and free-resources.html,
   replacing G-XXXXXXXXXX with your real ID:
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
   <script>
   window.dataLayer = window.dataLayer || [];
   function gtag(){dataLayer.push(arguments);}
   gtag('js', new Date());
   gtag('config', 'G-XXXXXXXXXX');
   </script>
4. Commit and push to GitHub.

Google Search Console setup
----------------------------
1. Go to search.google.com/search-console.
2. Add property: tinadoneit.com.au using Domain property (DNS verification,
   no meta tag needed).
3. Google will provide a TXT DNS record.
4. Add the TXT record in Cloudflare DNS.
5. There is no sitemap.xml for this 2-page site — Search Console will
   discover both pages via the internal link between them. If you'd
   rather submit URLs directly, use:
   https://tinadoneit.com.au/
   https://tinadoneit.com.au/free-resources.html

Booking tool setup
------------------
1. Create a free Calendly account.
2. Create an event type such as 'Free AI Discovery Call'.
3. Copy your Calendly link.
4. In both index.html and free-resources.html, find
   https://calendly.com/tinadoneit/30min and replace it with your
   actual booking link.

Contact links setup
--------------------
Both pages use mailto:hello@tinadoneit.com.au links, which open the
visitor's email app directly. For a professional production form
instead, connect one of these:
- Formspree
- Tally
- Basin
- Cloudflare Workers email handler

Suggested Upwork profile title
-------------------------------
AI Business Automation Consultant | WordPress | Shopify | ChatGPT | Cloudflare

Suggested Upwork profile intro
-------------------------------
Hi, I'm Faustina. I help businesses save time, reduce manual work and grow with AI-powered systems.

I combine business operations experience with practical AI automation, WordPress, Shopify, Cloudflare and process improvement to build systems that are easy to use, reliable and aligned with real business needs.

Key strengths:
- AI automation for customer enquiries, content, admin and follow-ups
- WordPress and Shopify websites with SEO, analytics and Cloudflare setup
- SOPs, workflow documentation and business process improvement
