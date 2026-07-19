# Pink First Website — Handoff Notes

## Project
Single-file HTML/CSS/JS nonprofit website for Pink First — a women's health awareness nonprofit that creates kits for women. Founded 2025 by Nitin Ponduri and Chirayu Pradhan (Nitin's mom had breast cancer, which inspired the idea).

## Files
- `D:\chishuan\pinkfirst\index.html` — entire website (HTML, CSS, JS all in one file)
- `D:\chishuan\pinkfirst\logo.png` — Pink First logo
- `D:\chishuan\pinkfirst\jade.jpg` — Jade Kamoun photo
- `D:\chishuan\pinkfirst\chirayu.jpg` — Chirayu Pradhan photo
- `D:\chishuan\pinkfirst\logos\` — university logos (12 schools)

## Local Preview
```
python -m http.server 3400 --directory D:/chishuan/pinkfirst
```
Open http://localhost:3400

## GitHub
https://github.com/kekoraa/PinkFirst

## Live Site
https://pinkfirst.org (Vercel, connected to GitHub)

## URGENT — Deployment Issue
Vercel is blocking all new deployments because the git commit email doesn't match a verified GitHub account. The live site is running the OLD version (still has the 2,400+ / 1,800+ hero stat cards). The local index.html is the correct updated version.

Fix to try:
```
npm i -g vercel
vercel --prod
```
This deploys directly from local files, bypassing the git email issue.

## Pushing Changes (once deployment works)
```
git add .
git commit -m "your message"
git push
```
Vercel auto-deploys on push.

## Pages
JS routing — showPage(pageId). Pages: home, about, programs, branches, donate, privacy, terms, accessibility

## Design
- Pink: #E8637A | Dark: #C94B63 | Light: #F9A8B8 | Pale: #FFF0F3 | Charcoal: #1A1A2E
- Fonts: Poppins (headings), Open Sans (body)

## Team (About page)
- Chirayu Pradhan — Co-Founder & CEO — chirayu.pradhan@tamu.edu — photo: chirayu.jpg
- Nitin Ponduri — Co-Founder & CEO — nponduri111@tamu.edu — SVG avatar (no photo)
- Jade Kamoun — CMO — jade.kamoun@utexas.edu — photo: jade.jpg

## Branches (14 schools)
UT Dallas, UT Austin, UCLA, Baylor, UW, Johns Hopkins, UNC, CU Boulder, Texas A&M, UC Riverside, Harvard, Rice, Case Western, UPenn

## Newsletter
Google Forms via fetch() no-cors
URL: https://docs.google.com/forms/d/e/1FAIpQLScjOLyjN8UyEy_mw8v_pzKpK3Fa4QyPZ4z4XxJQjen52aHB9Q/formResponse
Entries: 286226832 (first), 1730577509 (last), 523855388 (email), 1809582231 (phone)

## Donations
GoFundMe: https://gofund.me/b559a583f — single button, tiers are $5 / $15 / $25 (informational only)

## Contact
Email: pfirst@gmail.com | Phone: 346-754-1237 | Houston, TX
Instagram: https://www.instagram.com/pinkfirsttamu/

## What Was Changed from Original Template
- Removed: hero stat cards, volunteer section, testimonials, core values, pink stats bar, partner logos, "Request a Kit" button
- Updated: kit contents (real items), founding story, team members, donation amounts, vision/mission (women's health broadly)
- Added: partner inquiry form (mailto), 12 university logos, GoFundMe link
