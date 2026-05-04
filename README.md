# Refined Comfort Aesthetics — Website  

A high-performance, static marketing site for **Refined Comfort Aesthetics**, a boutique studio in New Braunfels, TX specializing in permanent hair removal, body contouring, and advanced facial sculpting.

**Live Site:** [comfortrefined.com](https://comfortrefined.com)

---

## 🛠 Tech Stack
This project is built for speed and maximum maintainability.
* **Core:** Vanilla HTML5, CSS3, and JavaScript.
* **Frameworks:** None (Zero build steps, no package managers).
* **Hosting:** [Cloudflare Pages](https://pages.cloudflare.com/) (Auto-deploys from `main` branch).
* **Integrations:** * **Booking:** Square Appointments Widget.
    * **Newsletter:** MailerLite (Inner Circle).
    * **Email:** forwardemail.net (Inbound routing).

---

## 📁 File Structure
* `index.html` — Home page (hero, services teaser, about, booking, footer).
* `services.html` — Full services list with collapsible details.
* `privacy-policy.html` — Privacy policy.
* `404.html` — Custom not-found page.
* `styles.css` — All shared styling (CSS custom properties at top).
* `sitemap.xml` — Submitted to Google Search Console.
* `robots.txt` — Allow-all plus sitemap pointer.
* `_headers` — Cloudflare Pages security and cache headers.
* `favicon.png` — Site favicon.
* `media/` — Photos and graphics referenced by the pages.

---

## 🚀 Making Changes & Deployment
Every push to the `main` branch triggers an automatic deployment. Changes are live in approximately 30 seconds.

### Common Edits:
| Task | How to do it |
| :--- | :--- |
| **Add a Service** | Copy a `service-category` block in `services.html` and update content/images. |
| **Change Pricing** | Search `services.html` for the specific dollar amount. |
| **Update Hours/Address** | Search `index.html` for the **JSON-LD schema** block (top) and the **footer**. |
| **Change Phone/Email** | Search all `.html` files for `5126607522` and `courtney@comfortrefined.com`. |

> **Note on Email:** Cloudflare's *Scrape Shield* is active. Plaintext email links are automatically encoded on the CDN to prevent spam.

---

## 💻 Local Preview
No build process is required. You can view changes locally using two methods:
1.  **Simple:** Open `index.html` directly in any web browser.
2.  **Server (Recommended):** Run the following command from the root folder:
    ```bash
    python3 -m http.server 8000
    ```
    Then visit `http://localhost:8000`.

*Note: The Square widget and MailerLite popup require an internet connection to load.*

---

## 📅 Booking Integration
The **Square Appointments** widget is embedded on `index.html` inside the `#booking` section. 
* **Source:** `https://square.site/appointments/buyer/widget/qkxy937f2kn11r/LTVFFJTEKVWGW.js`
* **Management:** Updates to the service menu, prices inside the widget, or staff availability are managed in the **Square Dashboard**, not this repository.

---

## ⚖️ License
All content, copy, photography, and branding **© Refined Comfort Aesthetics**. All rights reserved.
