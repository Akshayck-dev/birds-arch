# B.I.R.D. React architecture website

A responsive React + Vite implementation of the seven approved cream / forest green page designs. Real HTML, React components and local WebP photography assets, rather than flattened PNG pages.

## Run

Requires Node.js 20.19+ or 22.12+.

```bash
npm install
npm run dev
```

Open the URL printed by Vite. Production build:

```bash
npm run build
npm run preview
```

## Pages

Home, Projects (working category filters), Project Detail (six individual routes), Studio / Team, Expertise, Service Detail (five individual routes), Contact, plus a 404 screen. HashRouter keeps refresh/navigation working on static hosting without server rewrite rules. Example: `/#/expertise/interiors`.

## Customize

- `src/main.jsx`: project/service data, team, reusable components, all page content.
- `src/styles.css`: colors, typography, desktop/tablet/mobile layouts.
- `public/images/`: architectural photo regions extracted from the previously generated design mockups. These are AI concept images, not verified photographs of B.I.R.D. work. Replace with licensed real photography before public use.
- Brand/team/contact information follows the supplied website; descriptive copy and project narratives are illustrative and should be reviewed by the firm.

The inquiry form validates required fields and prepares a `mailto:` draft. It does not claim to submit enquiries to a server. Connect a server endpoint or email service for direct delivery. The phone and email links work. Instagram opens in a separate tab.

DM Sans is loaded from Google Fonts, with an Arial fallback if unavailable. All architectural images are bundled locally. For clean URLs and SEO-ready production rendering, switch HashRouter to BrowserRouter with hosting fallback rules or use a pre-rendering framework.
