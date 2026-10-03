# Bellure Clinic — Team Website

**Assignment #3 — Responsive Web Design (HTML and CSS only)**

| | |
|---|---|
| **Topic** | Medical cosmetology clinic in Astana |
| **Project goal** | Help a visitor understand the clinic's doctor-led approach, compare treatments and prices, meet the doctors, and prepare a consultation request. |
| **Live website** | https://aikonzhenisovvova-ops.github.io/bellure_clinic/ |
| **Repository** | https://github.com/aikonzhenisovvova-ops/bellure_clinic |
| **Group** | MT-2504 |

## Team and page ownership

| Member | GitHub | Page | Page-specific components |
|---|---|---|---|
| Nurakysheva Ayaulym | `aikonzhenisovvova-ops` | `index.html` — Home | Split hero, trust cards, six-item treatment grid, concern links, patient reviews |
| Bekbolat Adina | `adinabek` | `services.html` — Services | Category chips, three catalogue grids, scrollable price table, pre-visit checklist |
| Nazymkyzy Aizada | `Aizzadamsn` | `about.html` — About | Intro with "at a glance" card, team grid, visit timeline, values |
| Khabibullina Aigerim | `aigerim-kh` | `contact.html` — Contact | Demo booking form, contact card, treatment gallery, FAQ (`details`/`summary`) |

`demo-result.html` is a utility page opened by the demo form. It does not replace any of the four pages above. Shared work (header, footer, `style.css`, `responsive.css`, testing, deployment) was done by the whole team.

## How to open the project locally

1. Extract the ZIP.
2. Open `index.html` in any browser. All paths are relative, so no server is needed.

## Project structure

```
bellure-clinic/
  index.html  services.html  about.html  contact.html
  demo-result.html          form demonstration result page
  css/style.css             tokens, base rules, components (mobile first)
  css/responsive.css        min-width media queries
  images/                   SVG illustrations, logo mark, map
  fonts/                    self-hosted Fraunces and Manrope (woff2)
  README.md
```

## Responsive approach

- `style.css` describes the phone layout; `responsive.css` only adds layouts with `min-width` queries.
- Breakpoints: `48rem` (768px) and `64rem` (1024px), plus `90rem` (1440px) for a wider container.
- Navigation is a visible Flexbox menu that wraps onto extra rows on narrow screens.
- Wide content (the course price table) scrolls inside its own container; the page itself never scrolls sideways.

## Limitations of the static form

The contact form is a **demonstration only**. It uses native HTML validation (`required`, `type="email"`) and then opens `demo-result.html`. No data is sent, stored or delivered, and no confirmation of a booking is shown. A real booking form would need a server or form service and privacy rules for personal data, which are outside this assignment.

## Constraints followed

No JavaScript, no `<script>` tags, no inline event handlers, no inline styles, no CSS framework.
