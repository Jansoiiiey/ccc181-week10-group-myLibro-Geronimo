# CCC181 Week 10: CampusConnect Mobile-First Login Page

React + TypeScript starter for the Week 10 group activity. The page is already
built. Your group's job is the **mobile-first CSS** and the **GitHub teamwork**.

## Run it

```bash
npm install
npm run dev          # open the local URL it prints
npm run dev:phone    # same, but your phone (same Wi-Fi) can open the Network URL
npm run build        # must finish with no errors before you submit
```

## Rules

- Edit only the CSS files in `src/styles/` (one member = one file). Do not edit `reset.css`.
- Plain CSS only. No Tailwind, Bootstrap, Material UI, styled-components, or any UI library.
- Phone styles first (no media query), then `min-width` queries only. Never `max-width`.
- Do not edit the `.tsx` files or rename classes. If you must, tell the group first.

## Group information (fill in)

| Item | Your answer |
| --- | --- |
| Group number | |
| Section | |
| Repository URL | |

## Members (each member fills in their own row in their own commit)

| Member | Name | GitHub username | CSS file | What I did |
| --- | --- | --- | --- | --- |
| 1 (leader) | | | `base.css` | |
| 2 | Jonathan S. Geronimo Jr.|Jansoiiiey | `nav.css` | I edited src/styles/nav.css. On phones, the navbar uses Flexbox in a column with the brand on top and links stacked, all at least 48px tall with :hover and :focus-visible styles (--navy-hover and a gold outline), while the footer uses CSS Grid in one column with gold titles and 48px links. At 768px and up, the navbar becomes a row with the brand on the left and links on the right, and .nav-list lines up in one row. At 1024px and up, .footer-grid becomes three equal columns. Nothing changes at 1280px since .container (Member 1) handles centering. |
| 3 |  | | `form.css` | |

## Experiment 0: the page without the viewport tag

What did the page look like in DevTools phone mode **before** adding the viewport meta tag?
What changed **after** adding it?

> (write your answer here)

## DevTools test results

| Width | What must be true | Pass? |
| --- | --- | --- |
| 360 px | 1 column. Nav links stacked and 48px tall. Options and buttons stacked. Footer in 1 column. No sideways scrollbar. | |
| 768 px | Nav in one row (brand left, links right). Checkbox and link in one row. Two buttons side by side. | |
| 1024 px | Brand panel and login card side by side. Footer in 3 columns. Heading is larger. | |
| 1280 px | Content centered and stops at 1200px. | |

### Breakpoints I observed

Using **Show media queries** and dragging slowly from 360 px to 1280 px, the layout changed at these exact widths:

> Using Show media queries and dragging slowly from 360px to 1280px, the layout changed at exactly 768px and 1024px. At 768px, the navbar switched from a column to a row, with the brand on the left and the links in a single row on the right. At 1024px, the footer grid changed from one column to three equal columns. Nothing changed at 1280px. No width looked broken.

Screenshots are in `screenshots/` as `360.png`, `768.png`, `1024.png`, `1280.png`.

## What our group learned (leader writes this last)

> (write your answer here)
