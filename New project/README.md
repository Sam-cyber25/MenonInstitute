# The Institute — Menon

A static multi-page website for a legacy tuition institute in Kanpur, designed with an editorial and institutional visual language rather than a generic coaching-template look.

## Project Structure

```text
New project/
├── index.html
├── about/
│   └── index.html
├── classes/
│   └── index.html
├── contact/
│   └── index.html
├── subjects/
│   └── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── icons/
│   │   └── favicon.svg
│   └── js/
│       └── main.js
└── README.md
```

## Fonts Integration

The site uses Google Fonts with repeated `<link>` tags in every HTML page:

- `Cormorant Garamond` for headings and editorial emphasis
- `Jost` for body copy and interface text

## Design Notes

- Palette is restricted to:
  - `#1C3934` Te Papa Green
  - `#F4F8F9` Aqua Haze
  - `#C2A878` Muted Gold
  - `#1A1A1A` Charcoal Ink
- Layout uses borders and grid textures instead of heavy shadows.
- Motion is limited to subtle reveal-on-scroll, hover underline transitions, and a restrained mobile navigation toggle.
- The contact form opens a pre-filled WhatsApp enquiry to keep the site fully static and deployable without a backend.

## Local Preview

Because the navigation uses folder routes like `/about/` and `/classes/`, preview the site through a local web server instead of opening the files directly.

Examples:

```bash
# Python
python -m http.server 3000

# Node
npx serve .
```

Then open `http://localhost:3000`.

## Deploy on Vercel

1. Push this folder to a Git repository.
2. Import the repository into Vercel.
3. Set framework preset to `Other`.
4. Leave build command empty.
5. Leave output directory empty or set it to the repository root.
6. Deploy.

This site is fully static, so no server runtime is required.

## Deploy on Cloudflare Pages

1. Connect the repository to Cloudflare Pages.
2. Use no build command.
3. Set build output directory to `/`.
4. Deploy.

## Content Assumptions

The following public-facing details were used from current public listings and should be confirmed by the institute before launch:

- Address in Anand Bazar / Swaroop Nagar, Kanpur
- Public rating of `4.5`
- Timings: Monday to Friday `2:00 pm–8:00 pm`, Saturday `1:30 pm–7:00 pm`
- Phone number: `+91 93351 71404`
- update 1
