# Edits to your existing index.html (3 small changes)

Open index.html in your GitHub repo (pencil icon), make these three edits, then commit.

---

## Edit 1: add the nav link

FIND:
```html
<li><a href="#writing">Writing</a></li>
```
REPLACE WITH:
```html
<li><a href="#book">Book &amp; Tools</a></li>
<li><a href="#writing">Writing</a></li>
```

---

## Edit 2: add the book section

Paste this block directly ABOVE the line `<!-- WRITING -->`:

```html
  <!-- BOOK & TOOLS -->
  <section id="book" class="wrap">
    <div class="book-feature">
      <a href="/tools/" class="book-cover-link reveal" aria-label="The Blank Sheet Operator companion tools">
        <img src="/tools/images/book-cover.jpg" alt="Cover of The Blank Sheet Operator by Emmanuel C. Ikehi" loading="lazy" width="300" height="450">
      </a>
      <div class="reveal">
        <p class="eyebrow">New book</p>
        <h2 style="margin:0.7rem 0 1rem;">The Blank Sheet Operator</h2>
        <p class="lede" style="margin-bottom:1rem;"><em>Structuring, Pricing, and Delivering High-Value Ventures in Volatile Markets.</em></p>
        <p class="lede" style="margin-bottom:1.8rem;">How an operator takes an ambiguous opportunity, tests whether it deserves capital, models the economics, structures the deal, and decides whether to scale, pivot, pause, sell or kill. Eighteen chapters, each with a practical tool.</p>
        <div class="btn-row">
          <a href="/tools/" class="btn btn-solid">Free companion tools</a>
          <a href="https://amazon.com/author/emmanuelikehi" target="_blank" rel="noopener" class="btn btn-line">Get the book</a>
        </div>
      </div>
    </div>
  </section>
```

Then paste this CSS just ABOVE the closing `</style>` tag:

```css
  /* Book feature */
  .book-feature{ display:grid; grid-template-columns:260px 1fr; gap:4rem; align-items:center; border-top:1px solid var(--line); padding-top:4rem; }
  .book-cover-link img{ width:100%; height:auto; box-shadow:0 18px 40px rgba(23,25,22,0.28); transition:transform .25s ease; }
  .book-cover-link:hover img{ transform:translateY(-4px); }
  @media (max-width: 760px){ .book-feature{ grid-template-columns:1fr; gap:2rem; } .book-cover-link{ max-width:220px; } }
```

---

## Edit 3: add the book to your Writing list

Inside `<div class="writing-list">`, paste this as the FIRST row:

```html
      <div class="writing-row reveal">
        <div class="writing-title">
          <h3>The Blank Sheet Operator: Structuring, Pricing, and Delivering High-Value Ventures in Volatile Markets</h3>
          <span class="writing-meta">2026</span>
        </div>
        <a href="/tools/" class="link-arrow">Companion tools <span>→</span></a>
      </div>
```

---

## Optional tidy-ups

1. Your Amazon author links currently point to `https://amazon.com/author/emmanuelikehi`. The author page you gave me is:
   `https://www.amazon.com/stores/Emmanuel-C.-Ikehi/author/B0CYCQ3TV7`
   Use Find and Replace in your editor to swap it everywhere (it appears in the Writing section, the footer, and the new tools page). Once the book is live, link straight to its Amazon page instead.
2. On the Zyforix card, "ahead of a planned mainnet launch": update the wording if mainnet has launched or the date has changed. The book says the same, so keep the two consistent.
