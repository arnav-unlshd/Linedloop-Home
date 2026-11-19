# Lindenloop Home — GitHub Pages sample website

Lindenloop Home is a **fictional** Australian low-waste home-care brand built as a marketing-agent test site. It is not a shop and cannot accept real orders.

## Deploy to GitHub Pages (no build required)

1. Sign in to the GitHub account you want to use and create a **public** repository named `lindenloop-home` at https://github.com/new.
2. Upload **the contents of this folder** to the root of its `main` branch (so `index.html` lives at `/index.html`, not `/website/index.html`). Commit the files.
3. Open **Settings → Pages** in the repository. Under **Build and deployment**, choose **Deploy from a branch**, select `main`, directory `/ (root)`, and save.
4. Once GitHub Pages publishes, open `https://YOUR-USERNAME.github.io/lindenloop-home/` (replace YOUR-USERNAME with your GitHub login). Allow a little time for the first deployment.
5. Use that URL as the brand website in UNLSHD Flow.

Because all links and assets are relative, the pages work under a GitHub project-site path.

## What to test

- Landing page: `index.html` — brand, positioning and catalogue highlights.
- Shop: `shop.html` — five fictional products and demo cart events.
- Story: `story.html` — brand background and differentiation.
- Journal: `journal.html`, `journal-refills.html`, `journal-summer.html` — SEO/content surfaces.
- Campaigns: `campaigns.html` — sample creative angles and campaign links.
- Contact: `contact.html` — non-sending demo form.
- Event lab: `test-lab.html` — view/export simulated browser-only tracking events.

The demo pushes GA4-like events into `window.dataLayer` and keeps them in the browser's localStorage. It does **not** send analytics to any real analytics platform. It does not collect real orders or send forms/emails.

## Search indexing

The test website ships with `noindex,nofollow` and `robots.txt` disallowing crawlers, deliberately preventing a fictional ecommerce brand appearing as a real one in search results. To run real indexing experiments later, review the demo disclaimers and change both controls before submitting the URL to Search Console.

## Local preview

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000/.

## Customise

Edit the content in HTML files; edit design in `styles.css`. Icons and product art are in `assets/`. No build system, frameworks, authentication, payments or API keys are required.
