Tina Done It Version 3 Website
==============================

Email used on website: hello@tinadoneit.com.au

How to deploy on Cloudflare Pages
---------------------------------
1. Extract this ZIP file.
2. Upload all extracted files to your GitHub repository.
   Important: upload index.html, assets/, blog/, projects/, sitemap.xml and robots.txt directly.
3. In Cloudflare, go to Workers & Pages > Create > Pages > Connect to Git.
4. Select your GitHub repository.
5. Use these settings:
   - Framework preset: None
   - Build command: leave blank
   - Build output directory: /
6. Deploy.
7. Go to Custom Domains and add:
   - tinadoneit.com.au
   - www.tinadoneit.com.au

Google Analytics setup
----------------------
1. Create a GA4 property at analytics.google.com.
2. Copy your Measurement ID. It looks like G-XXXXXXXXXX.
3. Open index.html.
4. Replace both instances of G-XXXXXXXXXX with your real ID.
5. Commit/upload the updated file to GitHub.

Google Search Console setup
---------------------------
1. Go to search.google.com/search-console.
2. Add property: tinadoneit.com.au using Domain property.
3. Google will provide a TXT DNS record.
4. Add the TXT record in Cloudflare DNS.
5. After verification, submit sitemap:
   https://tinadoneit.com.au/sitemap.xml

Booking tool setup
------------------
1. Create a free Calendly account.
2. Create an event type such as 'Free AI Discovery Call'.
3. Copy your Calendly link.
4. In index.html, find https://calendly.com/ and replace it with your actual booking link.

Contact form setup
------------------
The current form uses mailto:hello@tinadoneit.com.au so it opens the visitor's email app.
For a professional production form, connect one of these:
- Formspree
- Tally
- Basin
- Cloudflare Workers email handler

Suggested Upwork profile title
------------------------------
AI Business Automation Consultant | WordPress | Shopify | ChatGPT | Cloudflare

Suggested Upwork profile intro
------------------------------
Hi, I'm Faustina. I help businesses save time, reduce manual work and grow with AI-powered systems.

I combine business operations experience with practical AI automation, WordPress, Shopify, Cloudflare and process improvement to build systems that are easy to use, reliable and aligned with real business needs.

Key strengths:
- AI automation for customer enquiries, content, admin and follow-ups
- WordPress and Shopify websites with SEO, analytics and Cloudflare setup
- SOPs, workflow documentation and business process improvement

