## Step 1 — Read the Room

Before writing a single line, understand what you're building and commit to a direction:

- **What is it**: What does this UI do? Who's actually using it?

- **Pick a vibe**: Go specific and commit — stark minimal, loud maximalist, retro-future, raw brutalist, high-end luxury, 
playful toy-like, editorial, art deco, soft pastel, industrial. One direction. Own it fully.

- **Tech boundaries**: Stack, performance constraints, accessibility needs.

- **The one thing**: What makes someone screenshot this?

Wishy-washy direction = forgettable output. Pick a lane and go all in.

Then ship code (HTML/CSS/JS, React, Vue, whatever) that is:
- Actually working, production-ready
- Visually distinct with a clear point of view
- Consistent from top to bottom
- Refined in every small detail

---

## Step 2 — The Visual Work

**Fonts**
Ditch Inter, Roboto, Arial — anything default. Find something with personality. Strong display font paired with a clean body font. Use negative tracking on large headers, positive on labels. Try lowercase italics instead of all-caps subheaders. Fix orphaned words with `text-wrap: balance`.

**Colors**
One accent. Not two, not three — one. Dominant palette with sharp contrast. Keep saturation under 80%. No pure `#000000` backgrounds — use off-blacks like `#0a0a0a` or dark tinted charcoals. Tint shadows to match the background hue instead of using black at low opacity. Use CSS variables for everything.

**Motion**
Make it count. One punchy page load with staggered reveals beats 20 micro-animations nobody notices. Hover states should surprise. Scroll triggers should feel earned. Use `transform` and `opacity` only — never animate `top`, `left`, `width`, `height`. Spring physics over linear easing wherever possible.

**Layout**
Break the grid. Asymmetry, overlaps, diagonal flow, deliberate spacing. Either generous whitespace or tight controlled density — nothing in between. No three equal card columns. No everything-centered symmetry. Use `min-height: 100dvh` not `100vh`. Add a max-width container (~1200-1440px). Let cards breathe or stack — never force equal heights with flexbox.

**Texture & Depth**
Skip flat solid backgrounds. Gradient meshes, noise overlays, geometric patterns, layered transparencies, deep tinted shadows, grain, decorative borders — whatever fits the vibe. True glassmorphism goes beyond blur: add a 1px inner border and subtle inner shadow. Spotlight borders that react to cursor. Broken grid elements that overlap and bleed.

---

## Step 3 — The Details That Actually Matter

**Content**
No "John Doe", no "Acme Corp", no round numbers like `99%` or `$100.00`. Use organic data: `47.2%`, `$94.00`, real-sounding names. No AI copywriting clichés — never write "Elevate", "Seamless", "Unleash", "Next-Gen", "Game-changer". Write plain, specific language. Sentence case on headers. Active voice always.

**States**
Every button needs hover, active, and focus states. `scale(0.98)` on press. 200-300ms transitions on everything interactive. Skeleton loaders not spinners. Empty states with actual design. Inline error messages — never `window.alert()`. Visible focus rings — not optional, it's accessibility.

**Components**
Cards only when elevation communicates hierarchy — not by default. Text links and tertiary buttons exist. No pill badges everywhere. No 3-card carousel testimonials. No accordion FAQs. No footer link farms. Squircle avatars over plain circles. Phosphor or Heroicons over Lucide/Feather defaults.

**Code**
Semantic HTML — `<nav>`, `<main>`, `<article>`, `<section>`. No inline styles mixed with classes. Relative units, not hardcoded pixels. Alt text on every meaningful image. Clean z-index scale. No Lorem Ipsum, no dead code, no `#` links, no import hallucinations.

**Easy wins people forget**
Custom 404 page. Legal links in footer. Form validation. Skip-to-content link. Proper meta tags — `<title>`, `description`, `og:image`. Favicon. Back navigation on every page. Cookie consent if needed.

---

## Step 4 — If Redesigning Existing Work

Don't rewrite from scratch. Work with what's there:

1. Font swap first — biggest instant win, lowest risk
2. Color cleanup — kill clashing or oversaturated colors
3. Add hover and active states — makes it feel alive
4. Fix layout and spacing — grid, max-width, consistent padding
5. Swap generic components for something less default
6. Add missing states — loading, empty, error
7. Polish typography scale last — the premium final touch

Rules: don't migrate frameworks, don't break existing functionality, check package.json before importing anything new, check Tailwind version (v3 vs v4) before touching config.

--

## What to Never Do

- Purple gradient on white background
- Space Grotesk as default font choice
- Three equal feature cards in a row
- Centered everything with perfect symmetry
- `box-shadow: 0 4px 6px rgba(0,0,0,0.1)` copy-paste shadows
- Generic Lucide icons for everything
- Lorem Ipsum anywhere
- `window.alert()` for errors
- Animating `top`, `left`, `width`, `height`
- Pure `#000000` or `#ffffff` backgrounds
- More than one accent color

--

