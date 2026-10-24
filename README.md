<html lang="en-IE">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Open Book Wednesdays · Mayor Street Library</title>
<meta name="description" content="Six Wednesday evenings. A reading list picked for you. A librarian who keeps talk on the book. €70, drink included. Starts Wednesday 4 November, 7pm, at Mayor Street Library.">
<meta name="theme-color" content="#14110e">

<!-- Open Graph / Twitter -->
<meta property="og:type" content="website">
<meta property="og:title" content="Open Book Wednesdays · Mayor Street Library">
<meta property="og:description" content="Finish the book. Actually talk about it. Six Wednesday evenings, a librarian-led list and a drink to finish. €70.">
<meta property="og:locale" content="en_IE">
<!-- og:image placeholder (1200x630, PNG or JPG, hosted at a public https URL). When you have it, add:
  <meta property="og:image" content="https://YOUR-DOMAIN/og-image.png">
  <meta property="og:image:width" content="1200">
  <meta property="og:image:height" content="630">
  <meta name="twitter:image" content="https://YOUR-DOMAIN/og-image.png">
-->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Open Book Wednesdays · Mayor Street Library">
<meta name="twitter:description" content="Finish the book. Actually talk about it. Six Wednesday evenings, a librarian-led list and a drink to finish. €70.">

<link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>📖</text></svg>">

<!--
  STILL TO DO (search for CONFIG in the script at the bottom):
  - og:image (see the comment above)
  - Optional: set CONFIG.bookingUrl to a booking page (Eventbrite, Ticket Tailor, etc.).
    While it is empty, the reserve button opens a pre-filled email to the library.
-->

<script>
/* Apply saved theme before first paint */
(function () {
  try {
    var t = localStorage.getItem("obw-theme");
    if (t === "light") document.documentElement.classList.add("light");
  } catch (e) {}
})();
</script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,600;0,700;1,500;1,600&family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&display=swap" rel="stylesheet">

<style>
:root {
  color-scheme: dark;
  /* Dark: warm charcoal and umber, muted brass */
  --bg: #14110e;
  --bg-grad: linear-gradient(170deg, #14110e, #1b1713 40%, #201b16 70%, #14110e);
  --glow: radial-gradient(ellipse 70% 42% at 50% 0%, rgba(194,164,107,0.09), transparent 70%);
  --surface: rgba(33,28,23,0.84);
  --border: rgba(196,167,112,0.22);
  --text: #e3dbcb;
  --text-bright: #f4eddf;
  --text-dim: #a39a88;
  --neon: #c2a46b;      /* muted brass */
  --cyan: #d6bd8a;      /* pale brass: links, focus */
  --green: #9fb19a;     /* faded sage */
  --amber: #c2a46b;

  --header-bg: rgba(20,17,14,0.7);
  --grid-line: rgba(196,167,112,0.03);
  --grain: 0.07;
  --orb-a: rgba(194,164,107,0.15);
  --orb-b: rgba(110,45,42,0.24);
  --cta-bg: #c2a46b;
  --cta-text: #1b1409;
  --amber-text: #d6bd8a;
  --spine-empty: rgba(163,154,136,0.09);
  --tool: rgba(205,175,112,0.72);
  --spine-icon: #e9d9b0;

  --display: "Cormorant Garamond", "Iowan Old Style", Garamond, Georgia, "Times New Roman", serif;
  --body: "EB Garamond", "Iowan Old Style", Garamond, Georgia, "Times New Roman", serif;
}

html.light {
  color-scheme: light;
  /* Light: bone, stone and parchment, muted oxblood */
  --bg: #eeeae0;
  --bg-grad: linear-gradient(170deg, #f1ede3, #ebe6d9 40%, #e6e0d1 70%, #f1ede3);
  --glow: radial-gradient(ellipse 70% 42% at 50% 0%, rgba(255,255,255,0.55), transparent 70%);
  --surface: rgba(251,248,241,0.86);
  --border: rgba(90,70,40,0.26);
  --text: #2d2b28;
  --text-bright: #171614;
  --text-dim: #5e5a52;
  --neon: #6b2b27;
  --cyan: #6b2b27;
  --green: #4a6048;
  --amber: #8a6a35;

  --header-bg: rgba(238,234,224,0.8);
  --grid-line: rgba(90,70,40,0.05);
  --grain: 0.06;
  --orb-a: rgba(194,164,107,0.22);
  --orb-b: rgba(130,70,60,0.12);
  --cta-bg: #6b2b27;
  --cta-text: #f6f1e6;
  --amber-text: #6b2b27;
  --spine-empty: rgba(90,70,40,0.07);
  --tool: rgba(196,163,98,0.85);
  --spine-icon: #efe2bc;
}

*, *::before, *::after { box-sizing: border-box; }
html { scroll-behavior: smooth; -webkit-text-size-adjust: 100%; }
body {
  margin: 0;
  font-family: var(--body);
  font-size: 19px;
  line-height: 1.7;
  color: var(--text);
  background-color: var(--bg);
  background-image: var(--glow), var(--bg-grad);
  background-attachment: fixed;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
  font-kerning: normal;
  overflow-x: clip;
  min-height: 100vh;
}
/* Paper grain */
body::before {
  content: ""; position: fixed; inset: 0; z-index: 0; pointer-events: none; opacity: var(--grain);
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='220' height='220'><filter id='n'><feTurbulence type='fractalNoise' baseFrequency='.85' numOctaves='2' stitchTiles='stitch'/><feColorMatrix values='0 0 0 0 .55 0 0 0 0 .5 0 0 0 0 .42 0 0 0 .6 0'/></filter><rect width='100%' height='100%' filter='url(%23n)'/></svg>");
}

/* Background layers */
.bg-grid {
  position: fixed; inset: 0; z-index: 0; pointer-events: none;
  background-image:
    linear-gradient(var(--grid-line) 1px, transparent 1px),
    linear-gradient(90deg, var(--grid-line) 1px, transparent 1px);
  background-size: 60px 60px;
}
.orb {
  position: fixed; z-index: 0; pointer-events: none;
  width: 380px; height: 380px; border-radius: 50%;
  filter: blur(60px);
}
/* Orbs sit outside the 880px content column */
.orb-a {
  top: 8%;
  right: calc(50% + 440px);
  background: radial-gradient(circle, var(--orb-a), transparent 68%);
  animation: orbitA 28s ease-in-out infinite;
}
.orb-b {
  top: 48%;
  left: calc(50% + 440px);
  background: radial-gradient(circle, var(--orb-b), transparent 68%);
  animation: orbitB 34s ease-in-out infinite;
}
@keyframes orbitA {
  0%   { transform: translate(0, 0); }
  25%  { transform: translate(-30px, 90px); }
  50%  { transform: translate(10px, 190px); }
  75%  { transform: translate(40px, 90px); }
  100% { transform: translate(0, 0); }
}
@keyframes orbitB {
  0%   { transform: translate(0, 0); }
  25%  { transform: translate(40px, -80px); }
  50%  { transform: translate(0, -170px); }
  75%  { transform: translate(-30px, -80px); }
  100% { transform: translate(0, 0); }
}

/* Header */
.site-header {
  position: sticky; top: 0; z-index: 50;
  background: var(--header-bg);
  -webkit-backdrop-filter: blur(20px);
  backdrop-filter: blur(20px);
  border-bottom: 1px solid var(--border);
}
.site-header .inner {
  max-width: 880px; margin: 0 auto; padding: 10px 24px;
  display: flex; align-items: center; justify-content: space-between; gap: 16px;
}
.brand {
  font-family: var(--display);
  font-size: 1.45rem; font-weight: 600; font-style: italic; letter-spacing: 0.005em;
  color: var(--text-bright); text-decoration: none; line-height: 1.1;
}
.brand span { color: var(--amber-text); }
.theme-toggle {
  display: inline-flex; align-items: center; justify-content: center;
  width: 40px; height: 40px; border-radius: 50%;
  border: 1px solid var(--border); background: var(--surface);
  color: var(--text-bright); cursor: pointer;
}
.theme-toggle svg { width: 19px; height: 19px; }
.theme-toggle .i-moon { display: none; }
html.light .theme-toggle .i-sun { display: none; }
html.light .theme-toggle .i-moon { display: block; }

/* Layout */
main, .site-footer { position: relative; z-index: 1; }
.wrap { max-width: 880px; margin: 0 auto; padding: 0 24px; }
section { padding: 52px 0; scroll-margin-top: 72px; }
h1, h2, h3 { font-family: var(--display); color: var(--text-bright); margin: 0; font-weight: 600; letter-spacing: -0.005em; }
h2 { font-size: clamp(2rem, 5vw, 2.7rem); line-height: 1.12; margin-bottom: 8px; }
.sec-head { text-align: center; margin-bottom: 32px; }
.kicker {
  display: block; font-family: var(--body); font-size: 0.8rem; font-weight: 500;
  letter-spacing: 0.26em; text-transform: uppercase; color: var(--amber-text); margin-bottom: 10px;
}
.sub { color: var(--text-dim); margin: 0; font-style: italic; font-size: 1.05rem; }
a { color: var(--cyan); text-underline-offset: 3px; }
:focus-visible { outline: 2px solid var(--cyan); outline-offset: 3px; border-radius: 2px; }

/* Ornamental divider */
.orn { display: flex; align-items: center; gap: 14px; max-width: 360px; margin: 8px auto; }
.orn span { flex: 1; height: 1px; background: linear-gradient(90deg, transparent, var(--border) 30%, var(--border) 70%, transparent); }
.orn i { width: 8px; height: 8px; border: 1px solid var(--amber-text); transform: rotate(45deg); flex: none; }

/* Hero */
.hero { padding: 76px 0 44px; text-align: center; }
.eyebrow {
  font-size: 0.82rem; font-weight: 500; letter-spacing: 0.28em; text-transform: uppercase;
  color: var(--amber-text); margin: 0 0 22px;
}
.hero h1 { font-size: clamp(2.9rem, 8.4vw, 5.2rem); line-height: 1.02; margin: 0 auto 24px; max-width: 14ch; font-weight: 600; }
.hero h1 em { font-style: italic; font-weight: 500; color: var(--amber-text); }
.hero .lead { font-size: 1.28rem; max-width: 600px; margin: 0 auto 32px; color: var(--text); }
.btn {
  display: inline-block; font-family: var(--body); font-weight: 500; font-size: 0.9rem;
  letter-spacing: 0.17em; text-transform: uppercase; line-height: 1.4; text-align: center;
  background: var(--cta-bg); color: var(--cta-text); text-decoration: none;
  padding: 15px 30px; border-radius: 2px; border: 1px solid var(--cta-bg); cursor: pointer;
  transition: transform .15s ease, box-shadow .15s ease;
}
.btn:hover { transform: translateY(-2px); box-shadow: 0 10px 26px rgba(0,0,0,0.28); }
.btn-ghost {
  background: transparent; color: var(--text-bright); border: 1px solid var(--border);
  padding: 13px 24px;
}
.btn-ghost:hover { box-shadow: none; border-color: var(--amber-text); }
.btn[disabled] { opacity: 0.4; cursor: not-allowed; transform: none; box-shadow: none; }
.small { font-size: 1rem; font-style: italic; color: var(--text-dim); margin: 20px 0 0; }

/* Cards (bookplate double frame) */
.card {
  position: relative; background: var(--surface); border: 1px solid var(--border);
  border-radius: 2px; padding: 28px;
}
.card::before {
  content: ""; position: absolute; inset: 6px; border: 1px solid var(--border);
  opacity: 0.55; pointer-events: none; border-radius: 1px;
}
.grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; }
.reason { text-align: center; }
.reason .num {
  font-family: var(--display); font-style: italic; font-weight: 500;
  font-size: 2.6rem; color: var(--amber-text); line-height: 1; margin-bottom: 12px;
}
.reason p { margin: 0; color: var(--text-bright); font-size: 1.1rem; }

/* Sample evening */
.steps { list-style: none; padding: 0; margin: 0 0 24px; display: grid; gap: 0; border-top: 1px solid var(--border); }
.steps li {
  border-bottom: 1px solid var(--border);
  padding: 16px 6px; display: flex; gap: 20px; align-items: baseline;
}
.steps .n { font-family: var(--display); font-style: italic; color: var(--amber-text); font-size: 1.6rem; min-width: 2.4ch; line-height: 1; }
.steps strong { font-weight: 600; color: var(--text-bright); }
.strip { margin-top: 22px; text-align: center; color: var(--text); }
.strip p { margin: 0; }
.strip p + p { margin-top: 6px; color: var(--text-dim); font-style: italic; }

/* Spines: antique leather and cloth, gold tooling */
.spines {
  display: flex; align-items: flex-end; justify-content: center; gap: 9px;
  padding: 18px 8px 4px; flex-wrap: nowrap; position: relative;
}
.spine-wrap { display: flex; flex-direction: column; align-items: center; gap: 8px; }
.spine {
  --c: #6e2d2a;
  position: relative;
  width: 34px; border-radius: 3px 3px 1px 1px;
  border: 1px solid var(--border);
  background: var(--spine-empty);
  color: var(--text-dim);
  transition: background .45s ease, color .45s ease, box-shadow .45s ease, border-color .45s ease;
}
.spine svg {
  position: absolute; top: 54%; left: 50%; width: 16px; height: 16px; transform: translateX(-50%);
}
.spine.on {
  background:
    linear-gradient(to bottom,
      transparent 0 9%, var(--tool) 9% 11%, transparent 11% 19%, var(--tool) 19% 20%,
      transparent 20% 78%, var(--tool) 78% 79%, transparent 79% 87%, var(--tool) 87% 89%, transparent 89%),
    repeating-linear-gradient(0deg, rgba(0,0,0,0.05) 0 1px, transparent 1px 3px),
    linear-gradient(90deg, rgba(0,0,0,0.38), rgba(255,255,255,0.08) 38%, rgba(0,0,0,0.05) 60%, rgba(0,0,0,0.34)),
    var(--c);
  border-color: rgba(0,0,0,0.4);
  color: var(--spine-icon);
  box-shadow: 0 5px 12px rgba(0,0,0,0.35), inset 0 0 0 1px rgba(255,255,255,0.04);
}
.spine.on::before {
  content: ""; position: absolute; left: 6px; right: 6px; top: 25%; height: 24%;
  border: 1px solid var(--tool); background: rgba(0,0,0,0.3); border-radius: 1px;
}
.spine-date { font-size: 0.78rem; letter-spacing: 0.08em; text-transform: uppercase; color: var(--text-dim); white-space: nowrap; }
.spine-gap {
  align-self: stretch; display: flex; flex-direction: column; align-items: center; justify-content: flex-end;
  gap: 8px; padding: 0 4px; min-width: 60px;
}
.spine-gap .line { flex: 1; border-left: 1px dashed var(--border); min-height: 60px; }
.spine-gap .lbl { font-size: 0.72rem; letter-spacing: 0.06em; font-style: italic; color: var(--text-dim); text-align: center; line-height: 1.2; }

/* Social proof */
blockquote { margin: 0; padding: 20px 4px 0; border-top: 1px solid var(--border); text-align: center; }
blockquote p {
  margin: 0 0 12px; font-family: var(--display); font-style: italic; font-weight: 500;
  font-size: 1.42rem; line-height: 1.32; color: var(--text-bright);
}
blockquote cite {
  font-style: normal; font-size: 0.78rem; letter-spacing: 0.2em; text-transform: uppercase; color: var(--text-dim);
}
.proof-closer { margin: 30px 0 0; text-align: center; color: var(--text); }

/* FAQ */
.faq details { border-top: 1px solid var(--border); }
.faq details:last-of-type { border-bottom: 1px solid var(--border); }
.faq summary {
  cursor: pointer; list-style: none; padding: 18px 4px; font-family: var(--display);
  font-size: 1.4rem; font-weight: 600; color: var(--text-bright); line-height: 1.25;
  display: flex; justify-content: space-between; gap: 16px; align-items: center;
}
.faq summary::-webkit-details-marker { display: none; }
.faq summary::after { content: "+"; color: var(--amber-text); font-size: 1.7rem; font-weight: 500; line-height: 1; flex: none; }
.faq details[open] summary::after { content: "–"; }
.faq .ans { padding: 0 4px 20px; margin: 0; color: var(--text); max-width: 700px; }

/* Qualifier */
.qualifier-card { padding: 32px; }
.q-meta { text-align: center; margin-bottom: 2px; }
.q-count { font-size: 0.8rem; letter-spacing: 0.26em; text-transform: uppercase; color: var(--amber-text); font-weight: 500; }
fieldset { border: 0; padding: 0; margin: 22px 0 0; min-width: 0; }
legend { font-family: var(--display); font-weight: 600; font-size: clamp(1.6rem, 4vw, 2.1rem); color: var(--text-bright); padding: 0; margin-bottom: 18px; line-height: 1.18; text-align: center; width: 100%; }
.opt { display: block; margin-bottom: 10px; cursor: pointer; position: relative; }
.opt input { position: absolute; opacity: 0; pointer-events: none; }
.opt .box {
  display: flex; gap: 16px; align-items: baseline; padding: 13px 18px; border-radius: 2px;
  border: 1px solid var(--border); background: transparent; color: var(--text);
  transition: border-color .15s ease, background .15s ease;
}
.opt .ltr { font-family: var(--display); font-style: italic; font-weight: 600; font-size: 1.35rem; color: var(--amber-text); min-width: 1.4ch; }
.opt:hover .box { border-color: var(--amber-text); }
.opt input:checked + .box { border-color: var(--amber-text); background: rgba(194,164,107,0.12); color: var(--text-bright); }
.opt input:focus-visible + .box { outline: 2px solid var(--cyan); outline-offset: 2px; }
.q-actions { display: flex; justify-content: space-between; gap: 12px; margin-top: 24px; }

/* Result */
.result { text-align: center; }
.result h3 { font-size: clamp(2.1rem, 6vw, 3.1rem); line-height: 1.08; margin-bottom: 18px; }
.result h3:focus { outline: none; }
.result .who { margin: 0 auto 14px; max-width: 620px; color: var(--text); }
.result .personal { margin: 0 auto 26px; max-width: 560px; color: var(--amber-text); font-family: var(--display); font-style: italic; font-weight: 500; font-size: 1.6rem; line-height: 1.25; }
.result .meta { margin: 12px auto 0; max-width: 620px; color: var(--text-dim); font-size: 1rem; }
.result .reads { margin: 22px auto 0; max-width: 620px; color: var(--text-bright); font-size: 1.08rem; }
.result .second { margin: 18px 0 0; color: var(--text); font-style: italic; }
.result .actions { margin-top: 24px; display: flex; flex-wrap: wrap; gap: 12px; align-items: center; justify-content: center; }
.result .foot { margin-top: 26px; padding-top: 20px; border-top: 1px solid var(--border); color: var(--text-dim); font-size: 1rem; }
.result .foot p { margin: 0 0 6px; }

/* Footer */
.site-footer { padding: 36px 0 56px; text-align: center; }
.site-footer .brand-line { font-family: var(--display); font-style: italic; font-size: 1.35rem; color: var(--text-bright); margin: 18px 0 8px; }
.site-footer .src { color: var(--text-dim); font-size: 0.92rem; font-style: italic; margin: 0 0 6px; }
.site-footer .contact { color: var(--text); font-size: 1rem; margin: 0 0 10px; }

[hidden] { display: none !important; }

@media (max-width: 720px) {
  body { font-size: 18px; }
  .grid-3 { grid-template-columns: 1fr; gap: 8px; }
  .hero { padding-top: 48px; }
  .spines { gap: 6px; }
  .spine { width: 26px; }
  .spine.on::before { left: 4px; right: 4px; }
  .spine-gap { min-width: 42px; }
  .qualifier-card { padding: 22px 18px; }
  .btn { padding: 14px 22px; }
}
@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  .orb { animation: none; }
  .btn, .spine { transition: none; }
}
</style>
</head>
<body>
<div class="bg-grid" aria-hidden="true"></div>
<div class="orb orb-a" aria-hidden="true"></div>
<div class="orb orb-b" aria-hidden="true"></div>

<header class="site-header">
  <div class="inner">
    <a class="brand" href="#top">Open Book <span>Wednesdays</span></a>
    <button class="theme-toggle" id="themeToggle" type="button" aria-label="Switch to light theme" title="Toggle light / dark theme">
      <svg class="i-sun" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="12" cy="12" r="4"/><path d="M12 2v2M12 20v2M4.9 4.9l1.4 1.4M17.7 17.7l1.4 1.4M2 12h2M20 12h2M4.9 19.1l1.4-1.4M17.7 6.3l1.4-1.4"/></svg>
      <svg class="i-moon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M21 12.8A9 9 0 1 1 11.2 3a7 7 0 0 0 9.8 9.8z"/></svg>
    </button>
  </div>
</header>

<main id="top">
  <div class="wrap">
    <!-- 1. HERO -->
    <section class="hero">
      <p class="eyebrow">Open Book Wednesdays · Mayor Street Library</p>
      <h1>Finish the book. <em>Actually talk about it.</em></h1>
      <p class="lead">Six Wednesday evenings. A reading list picked for you. A librarian who keeps talk on the book. A drink to finish.</p>
      <a class="btn" href="#qualifier">Find your cohort</a>
      <p class="small">€70 for all six evenings, drink included. Starts Wednesday 4 November, 7pm.</p>
    </section>

    <div class="orn" aria-hidden="true"><span></span><i></i><span></span></div>

    <!-- 2. THREE REASONS -->
    <section id="reasons" aria-labelledby="reasons-h">
      <div class="sec-head">
        <span class="kicker" aria-hidden="true">Chapter I</span>
        <h2 id="reasons-h">Three reasons this is for you</h2>
        <p class="sub">Six evenings, one list.</p>
      </div>
      <div class="grid-3">
        <div class="card reason"><div class="num">i.</div><p>There's no voting and no endless debate over what to read: a librarian picks each book, shaped by what your group enjoys.</p></div>
        <div class="card reason"><div class="num">ii.</div><p>A librarian runs the room, so the conversation stays on the book.</p></div>
        <div class="card reason"><div class="num">iii.</div><p>A fortnight between meetings gives you time to read, and €70 covers all six evenings, drink included.</p></div>
      </div>
    </section>

    <!-- 3. SAMPLE EXPERIENCE -->
    <section id="evening" aria-labelledby="evening-h">
      <div class="sec-head">
        <span class="kicker" aria-hidden="true">Chapter II</span>
        <h2 id="evening-h">A Wednesday evening, start to finish.</h2>
        <p class="sub">What an evening looks like.</p>
      </div>
      <ol class="steps">
        <li><span class="n">i.</span><span><strong>7pm, settle in</strong> with a group of readers.</span></li>
        <li><span class="n">ii.</span><span><strong>Discuss:</strong> your librarian opens with a question and keeps it on the book.</span></li>
        <li><span class="n">iii.</span><span><strong>Foyer:</strong> carry on talking over a drink, included.</span></li>
      </ol>
      <div class="card">
        <div class="spines" id="spinesStrip" role="img" aria-label="Six Wednesdays: 4 Nov, 18 Nov, 2 Dec, 16 Dec, 13 Jan, 27 Jan. No meeting on 30 December."></div>
      </div>
      <div class="strip">
        <p>Your six Wednesdays: 4 Nov · 18 Nov · 2 Dec · 16 Dec · 13 Jan · 27 Jan. No meeting on 30 December.</p>
        <p>Groups of 8 to 15 readers. If a stream is too full or too small, we'll place you in a different group.</p>
      </div>
    </section>

    <!-- 4. SOCIAL PROOF -->
    <section id="proof" aria-labelledby="proof-h">
      <div class="sec-head">
        <span class="kicker" aria-hidden="true">Chapter III</span>
        <h2 id="proof-h">What readers say about book clubs</h2>
        <p class="sub">Real frustrations, from real posts.</p>
      </div>
      <div class="grid-3">
        <blockquote><p>“organiser had no idea how to run one.”</p><cite>Mumsnet poster, c.2021</cite></blockquote>
        <blockquote><p>“it's just an excuse to get together and to drink wine really.”</p><cite>Mumsnet poster, c.2022</cite></blockquote>
        <blockquote><p>“A week is quite a short time for most people to read a book.”</p><cite>Mumsnet poster, 2025</cite></blockquote>
      </div>
      <p class="proof-closer">Almost 16 million visits to Irish public libraries in 2025 (LGMA). Mayor Street Library is next.</p>
    </section>

    <!-- 5. FAQ -->
    <section id="faq" class="faq" aria-labelledby="faq-h">
      <div class="sec-head">
        <span class="kicker" aria-hidden="true">Chapter IV</span>
        <h2 id="faq-h">Questions</h2>
        <p class="sub">The short answers.</p>
      </div>
      <details>
        <summary>I haven't read much lately. Will I keep up?</summary>
        <p class="ans">You're in good company: in Ireland, 40% of those surveyed read just one to five books a year (Red C for LGMA, 2026). You get two weeks to read each book, your first two books are set before the first night, and the library lends you the copy.</p>
      </details>
      <details>
        <summary>How are the books chosen?</summary>
        <p class="ans">A librarian picks each book, shaped by what your group enjoys. There's one assigned book for each evening, and the discussion stays on that book. Your first two are set before the first night. After that, your librarian suggests the next two titles ahead of time, just for fast readers who want to read ahead.</p>
      </details>
      <details>
        <summary>What if I haven't finished the book?</summary>
        <p class="ans">Come anyway. Before we start, everyone says how far they've got. Spoilers stay out of the room unless everyone has finished the book. Members who have finished can keep talking afterwards.</p>
      </details>
      <details>
        <summary>What does it cost?</summary>
        <p class="ans">€70 for all six evenings, drink included. That's about €11.70 an evening.</p>
      </details>
      <details>
        <summary>Do I need a library card?</summary>
        <p class="ans">Yes, and it's free. You borrow the book with your Mayor Street Library card. To get one, bring a valid ID and proof of address.</p>
      </details>
      <details>
        <summary>Why not join a free club?</summary>
        <p class="ans">Free clubs are great. This one adds a fixed run of six evenings, a list chosen for you and a librarian leading the room.</p>
      </details>
    </section>

    <div class="orn" aria-hidden="true"><span></span><i></i><span></span></div>

    <!-- 6. QUALIFIER -->
    <section id="qualifier" aria-labelledby="qual-h">
      <div class="sec-head">
        <span class="kicker" aria-hidden="true">Chapter V</span>
        <h2 id="qual-h">Find your cohort</h2>
        <p class="sub">Five questions. One stream.</p>
      </div>
      <div class="card qualifier-card">
        <noscript><p>The “Find your cohort” questions need JavaScript. Without it: the three streams are Crime &amp; Thriller, Romance &amp; Romantasy, and Contemporary &amp; Irish Fiction. To reserve a seat, email <a href="mailto:mayorstreetlibrary@dublincity.ie">mayorstreetlibrary@dublincity.ie</a>.</p></noscript>

        <div id="quiz" hidden>
          <div class="q-meta"><span class="q-count" id="qCount"></span></div>
          <div class="spines" id="spinesQuiz" role="img" aria-label=""></div>
          <form id="qForm" novalidate>
            <fieldset>
              <legend id="qText"></legend>
              <div id="qOpts"></div>
            </fieldset>
            <div class="q-actions">
              <button type="button" class="btn btn-ghost" id="qBack">Back</button>
              <button type="submit" class="btn" id="qNext" disabled>Next</button>
            </div>
          </form>
        </div>

        <div id="result" class="result" aria-live="polite" hidden></div>
      </div>
    </section>
  </div>
</main>

<!-- 7. FOOTER -->
<footer class="site-footer">
  <div class="wrap">
    <div class="orn" aria-hidden="true"><span></span><i></i><span></span></div>
    <p class="brand-line">Open Book Wednesdays at Mayor Street Library.</p>
    <p class="contact">Questions? <a href="mailto:mayorstreetlibrary@dublincity.ie">mayorstreetlibrary@dublincity.ie</a></p>
    <p class="src">Sources: Red C for LGMA, Ireland Reads (2026); NIQ, Irish Book Market (2026); LGMA (2026); Mumsnet posts.</p>
  </div>
</footer>

<script>
(function () {
  "use strict";

  /* ---------- CONFIG ---------- */
  var CONFIG = {
    // Leave empty to open a pre-filled email to the library. Set to a booking page URL
    // (Eventbrite, Ticket Tailor, etc.) once you have one and every reserve button will use it.
    bookingUrl: "",
    librarianEmail: "mayorstreetlibrary@dublincity.ie"
  };

  /* ---------- Theme toggle ---------- */
  var root = document.documentElement;
  var toggle = document.getElementById("themeToggle");
  function syncToggle() {
    var light = root.classList.contains("light");
    toggle.setAttribute("aria-label", light ? "Switch to dark theme" : "Switch to light theme");
    var meta = document.querySelector('meta[name="theme-color"]');
    if (meta) meta.setAttribute("content", light ? "#eeeae0" : "#14110e");
  }
  toggle.addEventListener("click", function () {
    root.classList.toggle("light");
    try { localStorage.setItem("obw-theme", root.classList.contains("light") ? "light" : "dark"); } catch (e) {}
    syncToggle();
  });
  syncToggle();

  /* ---------- Six spines ---------- */
  var DATES = ["4 Nov", "18 Nov", "2 Dec", "16 Dec", "13 Jan", "27 Jan"];
  var HEIGHTS = [76, 94, 84, 100, 88, 96];
  /* oxblood leather, faded slate blue, tobacco calf, old olive, chestnut, weathered teal */
  var COLORS = ["#6e2d2a", "#3b4a5c", "#7a5a3a", "#464f3c", "#5a3a2c", "#3d5a5c"];
  var GLASS = '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M7 3h10l-1 7a4 4 0 0 1-8 0L7 3z"/><path d="M12 14v7M8 21h8"/></svg>';

  function renderSpines(el, filled, withGap) {
    el.innerHTML = "";
    DATES.forEach(function (d, i) {
      if (withGap && i === 4) {
        var gap = document.createElement("div");
        gap.className = "spine-gap";
        gap.innerHTML = '<div class="line"></div><div class="lbl">No meeting<br>30 Dec</div>';
        el.appendChild(gap);
      }
      var wrap = document.createElement("div");
      wrap.className = "spine-wrap";
      var s = document.createElement("div");
      s.className = "spine" + (i < filled ? " on" : "");
      s.style.height = HEIGHTS[i] + "px";
      s.style.setProperty("--c", COLORS[i]);
      if (i === 5) s.innerHTML = GLASS;
      var lbl = document.createElement("div");
      lbl.className = "spine-date";
      lbl.textContent = d;
      wrap.appendChild(s);
      wrap.appendChild(lbl);
      el.appendChild(wrap);
    });
  }
  renderSpines(document.getElementById("spinesStrip"), 6, true);

  /* ---------- Qualifier data ---------- */
  var STREAMS = {
    C: {
      name: "Crime & Thriller",
      headline: "Your cohort: Crime & Thriller.",
      who: "Crime and thriller is the most popular genre across all demographics in Ireland (Red C for LGMA, 2026). If you like to guess, you'll like this room.",
      personal: {
        RETURNER: "Page-turners are the easiest way back into reading.",
        SOCIAL: "Bring your theories. Everyone else has one.",
        STRETCH: "We'll pick crime that rewards a close read."
      },
      cta: "Reserve my seat in Crime & Thriller",
      reads: [
        { t: "Lying in Wait", a: "Liz Nugent" },
        { t: "In the Woods", a: "Tana French" }
      ]
    },
    R: {
      name: "Romance & Romantasy",
      headline: "Your cohort: Romance & Romantasy.",
      who: "40% of Irish women pick up romance novels (Red C for LGMA, 2026). This is a room where that's the point, not a guilty pleasure.",
      personal: {
        RETURNER: "Stories you can't put down are how reading habits restart.",
        SOCIAL: "Come for the characters. Stay for the foyer drink.",
        STRETCH: "We'll push beyond the bestseller lists."
      },
      cta: "Reserve my seat in Romance & Romantasy",
      reads: [
        { t: "Book Lovers", a: "Emily Henry" },
        { t: "Caraval", a: "Stephanie Garber" }
      ]
    },
    L: {
      name: "Contemporary & Irish Fiction",
      headline: "Your cohort: Contemporary & Irish Fiction.",
      who: "Fiction hit a record mid-year share of the Irish print market in 2026 (NIQ). This is the room for the books everyone's talking about.",
      personal: {
        RETURNER: "A set list is the push to read the book you've been meaning to.",
        SOCIAL: "Good books, better arguments.",
        STRETCH: "Expect books you wouldn't pick yourself."
      },
      cta: "Reserve my seat in Contemporary & Irish Fiction",
      reads: [
        { t: "Small Things Like These", a: "Claire Keegan" },
        { t: "Brooklyn", a: "Colm Tóibín" }
      ]
    }
  };
  var ORDER = ["C", "R", "L"];
  var LETTERS = ["a.", "b.", "c.", "d."];

  /* pts = points per stream; primary = the single stream an answer points to (used for tie-breaks) */
  var QUESTIONS = [
    { q: "Which shelf do you head for first in a bookshop?", opts: [
      { t: "Crime & thriller", pts: { C: 3 }, primary: "C" },
      { t: "Romance, romantasy & fantasy", pts: { R: 3 }, primary: "R" },
      { t: "Literary & Irish fiction", pts: { L: 3 }, primary: "L" },
      { t: "A bit of everything", pts: {} }
    ]},
    { q: "What do you want most from a book?", opts: [
      { t: "A page-turner that keeps me guessing", pts: { C: 2 }, primary: "C" },
      { t: "An emotional ride", pts: { R: 2 }, primary: "R" },
      { t: "Great writing to chew on", pts: { L: 2 }, primary: "L" },
      { t: "Escape from my week", pts: { C: 1, R: 1 } }
    ]},
    { q: "What kind of book talk do you enjoy?", opts: [
      { t: "Theories: whodunnit, what's next", pts: { C: 2 }, primary: "C" },
      { t: "Favourite characters and moments", pts: { R: 2 }, primary: "R" },
      { t: "Themes and how it's written", pts: { L: 2 }, primary: "L" },
      { t: "Anything friendly", pts: {} }
    ]},
    { q: "How much reading time do you really have?", opts: [
      { t: "Evenings and weekends", pts: { L: 1 }, flag: "STEADY" },
      { t: "Little and often: commute, bedtime", pts: { C: 1, R: 1 }, flag: "LITTLE" },
      { t: "Not much right now", pts: { C: 1, R: 1 }, flag: "LITTLE" }
    ]},
    { q: "What are you hoping to get from six evenings?", opts: [
      { t: "A reason to read more", pts: {}, flag: "RETURNER" },
      { t: "People to talk books with", pts: {}, flag: "SOCIAL" },
      { t: "To be stretched by books I wouldn't pick", pts: {}, flag: "STRETCH" },
      { t: "A night out to look forward to", pts: {}, flag: "SOCIAL" }
    ]}
  ];

  var answers = [];   // chosen option index per question
  var idx = 0;

  var quiz = document.getElementById("quiz");
  var resultEl = document.getElementById("result");
  var form = document.getElementById("qForm");
  var qText = document.getElementById("qText");
  var qOpts = document.getElementById("qOpts");
  var qCount = document.getElementById("qCount");
  var qNext = document.getElementById("qNext");
  var qBack = document.getElementById("qBack");
  var spinesQuiz = document.getElementById("spinesQuiz");

  function esc(s) {
    return String(s).replace(/[&<>"]/g, function (c) {
      return { "&": "&amp;", "<": "&lt;", ">": "&gt;", '"': "&quot;" }[c];
    });
  }

  /* Reserve link: a booking page if set, otherwise a pre-filled email to the library */
  function bookingHref(stream) {
    if (CONFIG.bookingUrl) return CONFIG.bookingUrl;
    var subject = "Reserve my seat: " + stream.name + " (Open Book Wednesdays)";
    var body = "Hello,\n\nI'd like to reserve a seat in the " + stream.name +
      " cohort of Open Book Wednesdays, starting Wednesday 4 November at 7pm (€70 for six evenings).\n\n" +
      "Name:\nPhone:\nI already have a Mayor Street Library card (yes/no):\n\nThank you";
    return "mailto:" + CONFIG.librarianEmail + "?subject=" + encodeURIComponent(subject) + "&body=" + encodeURIComponent(body);
  }

  function updateSpines() {
    var filled = answers[idx] !== undefined ? idx + 1 : idx;
    renderSpines(spinesQuiz, filled, false);
    spinesQuiz.setAttribute("aria-label", filled + " of 5 questions answered");
  }

  function showQuestion() {
    var q = QUESTIONS[idx];
    qCount.textContent = "Question " + (idx + 1) + " of " + QUESTIONS.length;
    qText.textContent = q.q;
    qOpts.innerHTML = "";
    q.opts.forEach(function (o, i) {
      var label = document.createElement("label");
      label.className = "opt";
      var input = document.createElement("input");
      input.type = "radio";
      input.name = "q" + idx;
      input.value = i;
      if (answers[idx] === i) input.checked = true;
      input.addEventListener("change", function () {
        answers[idx] = i;
        qNext.disabled = false;
        updateSpines();
      });
      var box = document.createElement("span");
      box.className = "box";
      var ltr = document.createElement("span");
      ltr.className = "ltr";
      ltr.setAttribute("aria-hidden", "true");
      ltr.textContent = LETTERS[i];
      var txt = document.createElement("span");
      txt.className = "txt";
      txt.textContent = o.t;
      box.appendChild(ltr);
      box.appendChild(txt);
      label.appendChild(input);
      label.appendChild(box);
      qOpts.appendChild(label);
    });
    qNext.disabled = answers[idx] === undefined;
    qNext.textContent = idx === QUESTIONS.length - 1 ? "See my cohort" : "Next";
    qBack.style.visibility = idx === 0 ? "hidden" : "visible";
    updateSpines();
  }

  function score() {
    var s = { C: 0, R: 0, L: 0 };
    var flags = [];
    answers.forEach(function (a, qi) {
      var o = QUESTIONS[qi].opts[a];
      Object.keys(o.pts).forEach(function (k) { s[k] += o.pts[k]; });
      if (o.flag) flags.push(o.flag);
    });
    return { s: s, flags: flags };
  }

  function pickWinner(s) {
    var max = Math.max(s.C, s.R, s.L);
    var tied = ORDER.filter(function (k) { return s[k] === max; });
    if (tied.length === 1) return tied[0];
    for (var qi = 0; qi < 3; qi++) {               // tie-break: Q1, then Q2, then Q3
      var p = QUESTIONS[qi].opts[answers[qi]].primary;
      if (p && tied.indexOf(p) !== -1) return p;
    }
    return tied.indexOf("C") !== -1 ? "C" : tied[0]; // default: Crime & Thriller
  }

  function showResult() {
    var r = score();
    var win = pickWinner(r.s);
    var others = ORDER.filter(function (k) { return k !== win; })
      .sort(function (a, b) { return r.s[b] - r.s[a]; });
    var second = others[0];
    var showSecond = r.s[second] > 0 && (r.s[win] - r.s[second]) <= 1;

    var q5 = QUESTIONS[4].opts[answers[4]].flag;       // RETURNER | SOCIAL | STRETCH
    var st = STREAMS[win];

    var emailHtml = '<a href="mailto:' + esc(CONFIG.librarianEmail) + '">' + esc(CONFIG.librarianEmail) + "</a>";
    var readsHtml = st.reads.map(function (b) {
      return "<em>" + esc(b.t) + "</em> by " + esc(b.a);
    }).join(" and ");

    var html = "";
    html += '<h3 id="resultHead" tabindex="-1">' + esc(st.headline) + "</h3>";
    html += '<p class="who">' + esc(st.who) + "</p>";
    html += '<p class="personal">' + esc(st.personal[q5]) + "</p>";
    html += '<div class="actions"><a class="btn" id="ctaBtn" href="' + esc(bookingHref(st)) + '">' + esc(st.cta) + "</a></div>";
    if (!CONFIG.bookingUrl) html += '<p class="meta">This opens an email to Mayor Street Library with your stream filled in.</p>';
    html += '<p class="meta">€70 · six Wednesdays from 4 November, 7pm · drink included.</p>';
    html += '<p class="reads"><strong>Opening reads:</strong> ' + readsHtml + ".</p>";
    html += '<p class="meta">One book is assigned for each evening, and the discussion stays on that book. Your librarian also suggests the next two titles ahead, shaped by what your group enjoys, for fast readers who want to read ahead.</p>';
    if (showSecond) html += '<p class="second">Close second: <strong>' + esc(STREAMS[second].name) + "</strong></p>";
    html += '<div class="foot">';
    html += "<p>Groups are 8 to 15 readers. If a stream is too full or too small, we'll place you in a different group.</p>";
    html += "<p>Not sure? Ask a librarian: " + emailHtml + ".</p>";
    html += '<p style="margin-top:14px"><button type="button" class="btn btn-ghost" id="retake">Retake the questions</button></p>';
    html += "</div>";

    resultEl.innerHTML = html;
    quiz.hidden = true;
    resultEl.hidden = false;
    renderSpines(spinesQuiz, 6, false);

    document.getElementById("retake").addEventListener("click", restart);
    var head = document.getElementById("resultHead");
    head.focus({ preventScroll: true });
    document.getElementById("qualifier").scrollIntoView({ behavior: "smooth", block: "start" });
  }

  function restart() {
    answers = [];
    idx = 0;
    resultEl.hidden = true;
    resultEl.innerHTML = "";
    quiz.hidden = false;
    showQuestion();
    document.getElementById("qualifier").scrollIntoView({ behavior: "smooth", block: "start" });
  }

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    if (answers[idx] === undefined) return;
    if (idx < QUESTIONS.length - 1) { idx++; showQuestion(); }
    else showResult();
  });
  qBack.addEventListener("click", function () {
    if (idx > 0) { idx--; showQuestion(); }
  });

  quiz.hidden = false;
  showQuestion();
})();
</script>
</body>
</html>
