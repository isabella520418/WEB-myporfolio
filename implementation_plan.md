# Portfolio Design & Delivery Plan 

Hello there! It’s wonderful to collaborate with you on your new portfolio. As a designer, I always believe your portfolio should be an extension of your creative soul—it needs to balancing striking aesthetics, lovely typography, and rock-solid usability. 

Since we want full control over the visual harmony, we are going to rely on standard, beautiful **Vanilla HTML, CSS, and JS**. We won't let any bulky frameworks or utility-class clutter (like Tailwind) dictate our layout. This gives us the creative freedom to focus on the micro-interactions, rich gradients, and custom layouts that make a site truly memorable.

Let's dive into the blueprint for what we need to build!

## ✅ All Decisions Confirmed

| Decision | Choice |
|---|---|
| **Tech Stack** | Vanilla HTML, CSS, JS |
| **Layout** | Single-page scroll |
| **Projects** | 2–4 now, data-driven for easy additions later |
| **Vibe** | Soft & elegant |
| **Colors** | `#FFF1D3` Ivory · `#FFB090` Peach · `#CA5995` Magenta · `#5D1C6A` Deep Plum |
| **Heading Font** | Nunito |
| **Body Font** | Lato |
## Proposed Architecture and Changes

We will build the portfolio around a clean, modular file structure so it is easy to maintain.

### Core Foundation

The base layout and logic of the site.

#### [NEW] `index.html`
- This will be our single-page vessel (or the home layout if we expand). 
- We will use perfectly semantic HTML5 markup (e.g., `<header>`, `<main>`, `<section>`, `<footer>`).
- It will include sections for the **Hero (greeting & illustration)**, **Selected Work (gallery)**, **About Me**, and **Contact**.

#### [NEW] `styles/main.css`
- Our global style reset and layout engine using CSS Flexbox and Grid.
- We will define our design tokens here using CSS variables (CSS Custom Properties) for colors, typography, spacing, and transitions.

#### [NEW] `styles/components.css`
- To keep things tidy, we'll extract the styles for reusable elements into this file (e.g., buttons, cards for your projects, custom form inputs).

#### [NEW] `js/app.js`
- Vanilla JavaScript to handle any interactive elements. This includes smooth scrolling, a dynamic navigation bar that responds to scroll events, and subtle entrance animations for our sections as they come into view.

### Portfolio Content & Assets

We need beautiful imagery and structure to support your work!

#### [NEW] `assets/images/`
- Directory for your project thumbnails, profile picture, and any rich svg background patterns.
- *Wait, I don't have your projects yet!* We will generate a couple of stunning mockup placeholder images to get the UI feeling premium right off the bat.

#### [NEW] `data/projects.js` (Optional)
- We can store your portfolio project details (title, description, client, image path, tags) as a JSON/JS array here. This way, our `app.js` can dynamically render the portfolio grid without us copying and pasting HTML.

## Design Aesthetic — Soft & Elegant

*   **Color Palette:** Cream `#FFF1D3` as the primary background surface, deep plum `#5D1C6A` for headings & high-contrast text, magenta `#CA5995` as a sparingly used accent on CTAs and highlights, peach `#FFB090` for gentle hover states and decorative details.
*   **Typography:** Nunito (rounded, friendly, elegant) for all headings. Lato (humanist, very readable) for body copy. Generous line-heights and letter-spacing to keep things airy.
*   **Spacing & Layout:** Lots of breathing room — generous padding, a restrained max-width container, and a clean grid for project cards.
*   **Micro-animations:** Soft fade-in + upward drift on scroll reveal. Gentle scale & shadow lifts on card hover. Smooth colour transitions on nav links and buttons. No jarring or fast movements — everything should feel like a whisper.

## Page Sections (Single-Page Structure)

1. **Navigation** — Sticky top nav: logo/name on the left, anchor links on the right
2. **Hero** — Warm greeting, tagline, soft profile illustration, CTA button
3. **About** — Brief personal bio, key skills listed cleanly
4. **Work / Projects** — Responsive card grid (2–4 cards), data-driven via `data/projects.js`
5. **Contact** — Minimal contact form + social links
6. **Footer** — Copyright line

## Verification Plan

### Manual Verification
- Render the site via a local live server to review responsive behavior across desktop, tablet, and mobile.
- Verify color contrast for accessibility (WCAG standards are a must).
- Click through all navigation links and ensure smooth scroll transitions work flawlessly.
