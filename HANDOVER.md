# SEO + AEO + GEO Lead-Generation Funnel — Handover Report

Staging site only. No credentials are stored in this document.

## 1. Summary

| Item | Value |
|---|---|
| Landing page URL | https://darkgoldenrod-squid-772911.hostingersite.com/seo-aeo-geo-services/ |
| WordPress page name | **SEO, AEO & GEO Services** (Pages → All Pages, page ID 18) |
| Status | Published **on staging only** |
| Editing system | **Elementor** (already installed) using native widgets, plus **Fluent Forms** for the enquiry form |
| Page template | Elementor Canvas (no theme header/footer/menu, to remove distractions) |
| Lead storage | WordPress dashboard → **Fluent Forms → Entries** (form: "Visibility Enquiry Form", ID 3) |
| Lead notification email | **hello@growwithshuraim.com** (the site's WordPress admin email, via `{wp.admin_email}`) |

### Why Elementor
Audit found: Twenty Twenty-Five block theme (active), Elementor 4.3.6 Free (active), no form plugin, no SEO plugin, Privacy Policy page in *draft*. Elementor was already installed and gives visual, drag-and-drop editing of every heading, paragraph, button, icon, colour, font, spacing and background without touching code — so it was the best fit. Elementor Free has no form widget, so Fluent Forms (free) was added: it stores every entry in WordPress, sends email notifications, has spam protection and its own drag-and-drop form editor.

## 2. What was built (6 sections, in order)

1. **Hero** — eyebrow "SEO · AEO · GEO", H1, supporting paragraph, CTA "Get a Visibility Consultation" (scrolls to form), small context line.
2. **The Problem** — H2 + 3 problem cards with icons.
3. **The Solution** — H2 + 3 service cards (SEO, AEO, GEO) with icons + "Better together" concluding line.
4. **Enquiry Form** — H2, supporting line, "What happens next" list, Fluent Form (7 fields + privacy note + "Submit Enquiry"). Section anchor ID: `enquiry`.
5. **FAQ** — 5 accordion questions (one opens at a time) with automatic FAQ structured data.
6. **Final CTA** — dark section, H2, supporting copy, "Let's Talk" button (scrolls to form).

Design: warm off-white "paper" + white sections, deep ink headings in Fraunces (serif), Inter body text, a single emerald accent (#0B6E5B), thin-bordered cards with a subtle hover lift. No stock photos, fake stats, testimonials or logos.

## 3. Plugins / dependencies

| Plugin | Status | Why |
|---|---|---|
| Elementor (existing) | unchanged version | Page builder |
| **Fluent Forms 6.2.17** (free) | **newly installed** | Enquiry form, entry storage, notifications, spam protection |
| **Rank Math SEO 1.0.281** (free) | **newly installed** | SEO title, meta description, Service schema. Setup wizard: account connection was **skipped** (not required). |

Nothing paid was purchased. No theme change. No users changed.

## 4. Section-by-section editing guide (no code needed)

**Open the editor:** WordPress dashboard → Pages → hover "SEO, AEO & GEO Services" → **Edit with Elementor**.
Tip: open the **Navigator** (layers icon, or Ctrl/Cmd + I). Sections are named "1 — Hero", "2 — The Problem", … "6 — Final CTA".

General rules:
- **Edit text:** click any heading or paragraph on the page and type, or edit it in the left panel (Content tab).
- **Edit a button:** click it → Content tab → *Text* and *Link*. Keep the link as `#enquiry` to scroll to the form.
- **Change an icon:** click the icon → Content tab → *Icon* → choose from the library (or upload an SVG).
- **Styling of one element:** select it → **Style** tab (colour, font, size) and **Advanced** tab (spacing/margins, padding).
- **Section background / spacing:** select the section container in the Navigator → Style tab → Background; Advanced tab → Padding.
- **Hide an element on mobile/desktop:** select it → Advanced → *Responsive* → Hide on Desktop/Tablet/Mobile.
- **Images:** the page uses no images. To add one, drag an *Image* widget in and set **Alt text** in the Media Library.
- Always click **Publish/Update** (bottom-left) when done.

### Global colours & fonts (change once, updates the whole page)
In the editor: hamburger menu (top-left) → **Site Settings** → **Global Colors** / **Global Fonts**.
- Colours: *Brand Accent* (buttons, icons, eyebrows), *Ink (Headings)*, *Body Text*, *Accent Tint*, *Paper Background*, *White*, *Border*, *Dark Section*, *Accent Hover*, *Text on Dark*.
- Fonts: *Headings (Serif)* (all H2s), *Hero Headline (H1)*, *Card Title (H3)*, *Eyebrow Label*, *Body Text*, *Lead Paragraph*, *Button Text*, *Small Text* — each with desktop/tablet/mobile sizes.

### Hero
Navigator → "1 — Hero" → Hero Content: eyebrow (Heading widget), headline (Heading, H1), paragraph (Text Editor), Hero CTA → button + context list (Icon List — edit/add/remove the three items).

### Problem
"2 — The Problem": section header (eyebrow, H2, supporting text) and "Problem Cards" → Problem 1/2/3. Each card: Icon, title (Heading H3), description (Text Editor).

### Solution
"3 — The Solution": header, "Service Cards" → Service 1 — SEO / 2 — AEO / 3 — GEO. Each card: Icon, acronym (H3), full name (small label), description. The concluding "Better together" line is the last Text Editor in the section.

### Enquiry form (text around the form)
"4 — Enquiry Form" → Form Intro: eyebrow, H2, supporting line, "What happens next" (H3) and its 3-item list. The form card contains the **Fluent Forms** widget (form "Visibility Enquiry Form"). Its *Style* tab controls label/field/button colours, borders and spacing.

### FAQ
"5 — FAQ" → click the accordion.
- **Edit a question:** Content tab → Items → click the item → *Title*.
- **Edit an answer:** click the question on the canvas to open it, then click the answer text and edit.
- **Add:** Items → **+ Add Item** (then type the answer inside the new item).
- **Remove:** Items → hover item → trash icon. **Duplicate:** copy icon.
- **Reorder:** drag items up/down in the Items list.
- FAQ structured data updates automatically (Content → *FAQ Schema* is ON).

### Final CTA
"6 — Final CTA": heading, supporting text, "Let's Talk" button (link `#enquiry`).

## 5. Editing the enquiry form (fields, dropdown, messages, emails)

Dashboard → **Fluent Forms → Forms → "Visibility Enquiry Form" → Edit**.
- **Labels / placeholders / required / error messages:** click a field → right-hand "Input Customization" panel.
- **Dropdown options (Service Interested In):** click the dropdown → *Options* — add, remove, rename, reorder.
- **Add/remove fields:** drag from the left list; hover a field → trash icon to delete. Fields are in 2-column rows that stack on mobile.
- **Button text:** click the "Submit Enquiry" button in the editor.
- **Privacy note:** the small Custom HTML block above the button.
- **Success message:** Form → *Settings & Integrations* → **Confirmation Settings**.
- **Notification emails:** *Settings & Integrations* → **Email Notifications** → "New enquiry — admin notification". It sends to the site admin email, with *Reply-To* set to the visitor's email. Add more recipients here.
- Click **Save Form / Save Settings** after changes.

Spam protection (Fluent Forms → Global Settings → Miscellaneous): **Honeypot** and **Token-Based Spam Protection** are enabled. Optional extra: Global Settings → Security → Cloudflare Turnstile or reCAPTCHA (free keys required).

## 6. SEO / AEO / GEO configuration

- URL slug: `/seo-aeo-geo-services/`
- SEO title (Rank Math): *SEO, AEO & GEO Services for Google & AI Search Visibility*
- Meta description: *Get found by the right customers on Google and AI-powered search. Strategic SEO, AEO and GEO services for businesses. Request a visibility consultation.*
- Robots: index, follow. Canonical: self-referencing. Open Graph/Twitter tags via Rank Math.
- Headings: exactly one H1; H2 per section; H3 for cards, "What happens next" and FAQ questions.
- Structured data (verified in page source, no duplicates): WebSite, WebPage, **Service** (with SEO/AEO/GEO offer catalogue — edit in page editor → Rank Math → *Schema*), **FAQPage** (auto-generated from the Elementor accordion). Rank Math's default Article schema was replaced by Service. No ratings/reviews.
- Edit SEO title/description: Edit with Elementor → Rank Math icon (top of panel) or WordPress page editor → Rank Math box.

## 7. QA results (tested 6 Nov 2026)

| Check | Result |
|---|---|
| Desktop 1440px & mobile (iPhone 13) layouts | ✅ See `screenshots/` |
| Hero CTA & "Let's Talk" → scroll to form | ✅ Form lands at top of viewport (smooth scroll) |
| FAQ accordion (mouse + keyboard Enter) | ✅ One item open at a time |
| Empty submit | ✅ Custom inline errors for all 5 required fields |
| Invalid email / URL | ✅ Blocked with clear messages |
| Valid submission | ✅ Success message shown, form hidden |
| Lead storage | ✅ Entry #1 in Fluent Forms → Entries (all 7 fields + source URL) |
| Email notification | ✅ Fluent log: "Email Notification broadcasted to hello@growwithshuraim.com" — **inbox receipt not verifiable by me** |
| Spam protection | ✅ Automated (bot-like) submissions were rejected "Suspicious activity detected"; human-like submissions pass |
| Console errors | Only one: Hostinger Reach's sitewide `embed.js` was blocked in my test sandbox (not caused by this page) |
| Colour contrast (WCAG AA) | ✅ Button 6.2:1, body text 7.3:1, dark section 11.3:1 |
| Keyboard focus | ✅ Visible focus ring on buttons; emerald border + ring on inputs |
| Performance | ~31 requests, FCP ≈ 1.3 s, load ≈ 2.1 s (from test location); no images |

The test entry is named "QA Test — please ignore" — delete it from Fluent Forms → Entries whenever you like.

## 8. Rollback point

Before changes: full WXR export (Tools → Export equivalent), plus a record of plugins, settings, theme and the default Elementor kit. To undo everything: delete page ID 18, deactivate/delete Fluent Forms and Rank Math, and reset Elementor Site Settings → Global Colors/Fonts (previous values were Elementor defaults: Roboto / Roboto Slab, #6EC1E4, #54595F, #7A7A7A, #61CE70).

## 9. Limitations & actions needed from you

1. **Check your inbox** (and spam folder) at hello@growwithshuraim.com for "New visibility enquiry from QA Test…". Hostinger uses PHP mail by default; for reliable delivery install a free SMTP plugin (e.g. FluentSMTP) with your mailbox's SMTP details.
2. **Privacy Policy is still a draft.** Once you publish it, add a link in the form's privacy note (Fluent Forms → form → Custom HTML block). It was not linked to avoid a broken link.
3. **Business name is not set.** Settings → General → *Site Title* is currently the staging domain, which Rank Math uses as the Organization name in schema. Set your real business name there, and in Rank Math → Titles & Meta → Local SEO add the logo/name.
4. **Duplicate `<title>` tag:** Elementor Canvas on a block theme prints the title twice (both identical, so the SEO impact is minimal). Fixing it requires a theme switch (e.g. Hello Elementor) or a code snippet — not done, to avoid global changes.
5. **No footer/menu by design** (Canvas). Add a small footer with your business details & privacy link once available.
6. **Fonts load from Google**; optional: Elementor → Settings → Performance → *Google Fonts: Load Locally*.
7. No internal links were added because the site has no other published pages yet.
8. Hostinger Reach's `embed.js` loads sitewide (unrelated to this page).
9. LiteSpeed Cache is active — after editing, use the admin bar **LiteSpeed → Purge All** if changes don't appear for logged-out visitors.
