# Day 1: Visual Regression & Layout Diagnostics

## What I did

Performed a manual UI audit of the Amazon search results page for the query "toys for ages 5-7". The goal was to check how well the page looks, how it responds when you resize the browser window, and whether the shopping cart updates correctly in real time.

**Page tested:** [Amazon — Toys for Ages 5-7](https://www.amazon.com/s?k=toys+for+ages+5-7&ref=sr_nr_p_rag_integrated_qb_1)

---

## What I found

### Things that work well

| What I tested | What I saw | Why it matters |
|---|---|---|
| Price display | The cents are shown smaller and bold (e.g. $16.**97**) | Makes prices easier to scan quickly |
| Shopping cart | Cart count updates instantly when you add an item | Shows the site keeps your session data correctly |
| Trust badges | "Best Seller" and "Overall Pick" labels are clearly visible | Helps users make decisions faster |

---

### Problems I found

| Problem | What happens | Risk level |
|---|---|---|
| Grid layout breaks on resize | Product cards lose alignment when you drag the browser window smaller | High — layout looks broken on tablets |
| Product titles are too long | Titles are stuffed with keywords and hard to read | High — likely to overlap or get cut off on mobile screens |
| Mobile layout risk | Combination of misaligned cards + long titles = components overlapping on small screens | High — mobile users would have a poor experience |

---

## Skills used

- Manual visual regression testing
- Responsive layout and breakpoint testing
- Bug documentation and severity rating

---

## Key takeaway

The page has solid foundations — pricing, cart, and trust badges all work well. But the layout is fragile under viewport changes and the product titles create a real risk of broken layouts on mobile. These issues should be fixed before a production release.
