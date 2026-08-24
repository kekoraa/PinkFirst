# Pink First

Pink First is a nonprofit dedicated to breast cancer awareness and women's health. Founded in 2025 by Nitin Ponduri and Chirayu Pradhan, the organization assembles and distributes women's health kits to women in need through a network of student-led college campus branches.

**Live site:** [pinkfirst.org](https://pinkfirst.org)

## Tech Stack

Plain HTML, CSS, and JavaScript — no build step, no frameworks, no dependencies. Everything (markup, styles, and scripting) lives in a single `index.html` file, with page navigation handled client-side via a JS router (`showPage(pageId)`).

## Project Structure

```
index.html      Entire website — HTML, CSS, and JS
logo.png        Pink First logo
chirayu.jpg     Team photo — Chirayu Pradhan
jade.jpg        Team photo — Jade Kamoun
logos/          University branch logos (16 schools)
```

## Pages

Home, About, Programs, Branches, Donate, Privacy, Terms, Accessibility — all rendered from `index.html` and switched via client-side routing (no page reloads).

## Running Locally

```
python -m http.server 3400 --directory .
```

Then open [http://localhost:3400](http://localhost:3400).

## Deployment

Hosted on [Vercel](https://vercel.com), connected to this GitHub repo. Pushes to the main branch auto-deploy:

```
git add .
git commit -m "your message"
git push
```

## Features

- **Branches** — 16 university chapters, each with a logo, name, and location
- **Newsletter signup** — submits to Google Forms via a `fetch()` POST
- **Partner inquiry form** — collects a name, email, and message
- **Donations** — links out to GoFundMe

## Design

| Token | Value |
|---|---|
| Pink | `#E8637A` |
| Dark | `#C94B63` |
| Light | `#F9A8B8` |
| Pale | `#FFF0F3` |
| Charcoal | `#1A1A2E` |

Fonts: [Poppins](https://fonts.google.com/specimen/Poppins) (headings), [Open Sans](https://fonts.google.com/specimen/Open+Sans) (body).

## Contact

- Email: pinkfirstnpo@gmail.com
- Phone: 346-754-1237
- Location: Houston, TX
- Instagram: [@pinkfirsttamu](https://www.instagram.com/pinkfirsttamu/)
