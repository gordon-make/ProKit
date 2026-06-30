# PROKIT

**專業球衣及團隊衫訂製** — A single-page marketing site for PROKIT Teamwear Studio, showcasing custom jersey design, production workflow, and sample work.

## Overview

PROKIT is a static landing page built for Hong Kong–based teamwear customization. It highlights:

- Full sublimation printing and geometric panel designs
- Sponsor logos, custom fonts, and name/number personalization
- Reference samples (player kits and goalkeeper kits)
- A four-step production workflow from design to delivery
- WhatsApp and inquiry form contact options

The site uses **Traditional Chinese (zh-HK)** copy and a dark, sports-focused visual style.

## Project Structure

```
PROKIT/
├── index.html      # Main landing page (all content in one file)
├── New Jer.jpg     # Sample image — Orion player kit (optional)
├── GK_Jersey.jpg   # Sample image — goalkeeper dragon kit (optional)
└── README.md
```

## Requirements

- A modern web browser
- Internet access (Tailwind CSS is loaded from CDN)
- No Node.js, build tools, or server required

## Getting Started

1. Clone or copy this folder to your machine.
2. Add sample images to the same directory as `index.html`:
   - `New Jer.jpg` — Orion grey/blue geometric player kit
   - `GK_Jersey.jpg` — Black/gold goalkeeper dragon pattern kit
3. Open `index.html` in a browser (double-click or drag into the browser window).

If images are missing, the page still loads; placeholder messages appear in the sample cards instead.

### Local preview (optional)

From the project folder:

```bash
# Python 3
python -m http.server 8080

# Then open http://localhost:8080
```

## Page Sections

| Section | ID | Description |
|---------|-----|-------------|
| Navigation | — | Sticky header with links and WhatsApp CTA |
| Hero | — | Main headline and primary call-to-action |
| 工藝細節 | `#services` | Core capabilities (sublimation, panels, sponsors) |
| 實物範例 | `#samples` | Product sample cards with images |
| 製作流程 | `#process` | 4-step workflow (design → production → QC → delivery) |
| 聯絡/報價 | `#contact` | WhatsApp link and inquiry form |

## Tech Stack

- **HTML5** — semantic structure
- **Tailwind CSS** (CDN) — layout and styling
- **Vanilla JavaScript** — minimal (form submit placeholder, image fallback)

## Customization

### Contact / WhatsApp

WhatsApp links use phone number `85251309781`. Search `51309781` or `api.whatsapp.com` in `index.html` to update.

### Inquiry form

The contact form currently shows a success alert on submit and does not send data anywhere. To connect it to a backend or service (e.g. Formspree, Google Sheets, email API), replace the `onsubmit` handler on the `<form>` element.

### Sample images

Replace or add images by editing the `<img src="...">` tags in the `#samples` section. Keep files in the same folder as `index.html`, or use full/relative paths as needed.

### Styling

Custom hover effects are defined in the `<style>` block in `<head>`. Most layout and colors use Tailwind utility classes inline.

## Browser Support

Works in current versions of Chrome, Firefox, Safari, and Edge. Responsive layout uses Tailwind breakpoints (`sm`, `md`, `lg`).

## License

© 2026 PROKIT Teamwear Studio. All rights reserved.
