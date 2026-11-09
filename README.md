# Next Level Gaming & Esports Arena

**Student:** Brian Mupataie  
**Student number:** ST10526359  
**Module:** WEDE5020 Web Development (Introduction)  
**Repository:** https://github.com/ST10526359/Next-Level-Gaming-Esports-Arena  
**GitHub Pages:** https://st10526359.github.io/Next-Level-Gaming-Esports-Arena/

## Project overview
This repository contains the final web-development implementation for the Next Level Gaming and Esports Arena student project. The concept is based in Johannesburg and is aimed at gamers, esports players, families, birthday groups, schools and work teams.

The website is an educational demonstration and is **not** an official business booking or payment system.

## Part 2 fixes carried into the final version
- Keeps the responsive dark-blue / bright-blue / purple / green visual direction.
- Keeps the package and experience information from the earlier proposal.
- Keeps the fee calculator and discount rules.
- Improves semantic HTML and heading structure.
- Separates the general contact form and package enquiry form into their own pages.
- Improves navigation for desktop and mobile.
- Adds accessible labels, status messages and image alt text.
- Documents unverified/illustrative prices instead of presenting them as confirmed business prices.

## Part 3 JavaScript functionality
- **Dynamic content loading:** activities are loaded with `fetch()` from `data/activities.json`, with a fallback list if loading fails.
- **Search and filtering:** users can search activities by text and filter between all items, packages and single experiences.
- **Modal:** each activity has a “View details” button that opens a modal dialog.
- **Tabs:** All / Packages / Experiences category controls.
- **Accordion:** FAQ sections expand and collapse.
- **Lightbox:** gallery images open in a full-screen lightbox.
- **Interactive map:** the Contact page uses Leaflet with OpenStreetMap tiles and a Johannesburg reference marker.
- **Fee calculator:** selected activities are totalled dynamically and the 5% / 10% / 15% discount rules are applied.
- **Responsive navigation:** the mobile menu opens and closes with JavaScript.

## Forms and AJAX
Two separate forms are included:
1. `enquiry.html` — package / activity enquiry form.
2. `contact.html` — general contact form.

Both forms use HTML5 required fields and input types, JavaScript validation through `checkValidity()` / `reportValidity()`, accessible live status messages, and AJAX submission with the Fetch API.

For assessment demonstration, AJAX requests are sent to **JSONPlaceholder**, a public test API. No real booking or business message is created. Users should not enter sensitive information.

## SEO implementation
- Unique page titles and page-specific meta descriptions.
- Canonical links and robots meta tags.
- Semantic heading structure.
- Descriptive navigation text and image `alt` text.
- `robots.txt` and `sitemap.xml`.
- Responsive/mobile-friendly layout.

## File organisation
```
Next-Level-Gaming-Esports-Arena/
├── index.html
├── enquiry.html
├── contact.html
├── style.css
├── script.js
├── forms.js
├── robots.txt
├── sitemap.xml
├── data/
│   └── activities.json
└── images/
    ├── esports.svg
    ├── vr.svg
    └── racing.svg
```

## Content research and sourcing
The website content is based primarily on the student's earlier Next Level Gaming proposal. The R1 500 Ultimate Gamer Pass price comes from that proposal. Other package/experience prices remain clearly labelled as illustrative demo values because verified business pricing was not supplied.

Original SVG illustrations in the `images` folder were created specifically for this project. The interactive map uses OpenStreetMap data through Leaflet.

## Changelog
### 9 November 2026 — POE Part 3 finalisation
- Expanded README with implementation details, changelog and references.
- Added `enquiry.html` and `contact.html`.
- Added HTML5 and JavaScript form validation.
- Added AJAX demo submissions.
- Added JavaScript search/filtering, tabs, modal, accordion and lightbox.
- Added dynamic JSON content loading.
- Added an interactive Leaflet/OpenStreetMap map.
- Added SEO metadata, alt text, `robots.txt` and `sitemap.xml`.
- Improved responsive styling and accessibility.
- Preserved the fee calculator and project colour palette.

## Testing checklist
- Open Home, Enquiry and Contact pages.
- Test the mobile navigation at a narrow browser width.
- Search and filter activities.
- Open and close an activity modal.
- Open and close each FAQ accordion.
- Open all gallery images in the lightbox.
- Select 1, 2, 3 and 4+ activities and confirm the discount calculations.
- Submit each form with missing fields to verify validation.
- Submit each valid form to verify the AJAX status message.
- Zoom and move the interactive map.
- Confirm `robots.txt` and `sitemap.xml` load from the deployed site.

## References
- MDN Web Docs. Fetch API: https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API
- MDN Web Docs. Client-side form validation: https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Form_validation
- Google Search Central. SEO Starter Guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- Leaflet. JavaScript library for interactive maps: https://leafletjs.com/
- OpenStreetMap. Map data: https://www.openstreetmap.org/
- JSONPlaceholder. Fake REST API for testing: https://jsonplaceholder.typicode.com/
