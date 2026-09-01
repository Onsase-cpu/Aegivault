# Cartivex Design Direction

## Three stylistic approaches

### Theme Name: Signal Market
Very Brief Intro: A confident editorial commerce system that treats products like signals in a living marketplace: bright orange actions, botanical green trust cues, and blue operational structure against ink-black contrast.
Probability: 0.07

### Theme Name: Field Notes Commerce
Very Brief Intro: A tactile, paper-led shopping experience with warm neutrals, stamped details, and a slower, more considered rhythm inspired by independent makers.
Probability: 0.03

### Theme Name: Orbit Ledger
Very Brief Intro: A dark operational dashboard language with electric accents, dense data layers, and motion-led navigation for a commerce platform built for scale.
Probability: 0.08

## Chosen approach: Signal Market

### Design Movement
Contemporary editorial brutalism with the clarity of Swiss information design and the warmth of African independent-market commerce.

### Core Principles
1. Make every screen feel like a confident market instrument: decisive type, clear hierarchy, and direct actions.
2. Pair rigid information structures with organic color blocks and soft paper-like surfaces.
3. Prefer asymmetric composition and layered panels over centered, generic SaaS layouts.
4. Treat microcopy as product guidance, not filler: every label should reduce uncertainty.

### Color Philosophy
Near-black creates authority and allows the chromatic system to read as functional signals. Orange means momentum and action; green means verified value, fulfillment, and trust; blue means navigation, infrastructure, and operational clarity. The palette should feel energetic without becoming neon or childish.

### Layout Paradigm
Use a left-weighted editorial rail, oversized lead statements, offset product cards, and dashboard-style data strips. Public storefront screens should feel like a magazine spread with commerce mechanics attached; admin screens should use an anchored sidebar and wide working canvas.

### Signature Elements
1. Offset orange signal bars and corner notches used to mark active states.
2. Product cards with slightly irregular image frames and large editorial captions.
3. Thin blue rules and green status chips used as a visual operating language.

### Interaction Philosophy
Interactions should confirm intent quickly and visibly. Buttons compress on press, cards lift minimally on hover, filters slide from the edge, and cart changes update with a brief signal pulse. Avoid decorative motion that competes with shopping decisions.

### Animation
Use 160–240ms ease-out transitions for hover, drawer, and filter states. Stagger product entrances by 40ms. Use a short orange pulse when an item enters the cart. Respect prefers-reduced-motion and keep keyboard navigation instantaneous.

### Typography System
Use Space Grotesk for display and navigation, paired with IBM Plex Sans for body and utility text. Headlines use tight tracking and strong weight contrast; product names use medium weight; metadata uses uppercase IBM Plex Sans with generous tracking. Never use Inter.

### Brand Essence
Cartivex is commerce infrastructure for ambitious modern storefronts, built for teams who want clarity from catalog to checkout without sacrificing character. Personality: **decisive, tactile, connected**.

### Brand Voice
Headlines are short, specific, and a little kinetic. CTAs name the next action. Microcopy anticipates hesitation and resolves it in plain language.

Example lines:
- “A better way to move product.”
- “Add it to the flow.”

### Wordmark & Logo
The mark is a compact four-cell interlock: two orange cells and one green cell orbit a blue negative-space notch, suggesting products, systems, and movement. The wordmark is set in a custom-spaced Space Grotesk treatment with the “x” slightly raised as a signal marker; the logo graphic is used independently as the favicon and mobile app icon.

### Signature Brand Color
Cartivex Signal Orange — `#F05A28` — an ownable, warm orange that reads as action on near-black and as a confident editorial accent on parchment surfaces.

## Implementation guardrails

This MVP is intentionally frontend-only and JavaScript-only. It will use local seed data and localStorage for cart and order state, while documenting where the REST API, authentication, database, payments, and search layers from the architecture brief should connect. It will not fabricate customer reviews or testimonials. It will not include AI labels, watermarks, badges, or vendor-specific folder names.

## Style Decisions

- The orange bar/notch, thin blue rule, and green status chip are a repeated system on every major surface: orange marks action and momentum, blue marks navigation and operational structure, and green is reserved for trust, fulfillment, and verified value.
- Product cards use offset image frames, larger editorial captions, and uppercase IBM Plex Sans metadata so the catalogue reads as a considered edit rather than generic inventory.
- The Cartivex wordmark includes the raised orange “x” signal treatment and is paired with the interlock mark in header and footer contexts.

# Aegivault App Direction

## Chosen approach: Night Operations Console

Aegivault deliberately moves away from Cartivex's warm editorial commerce language. It uses a dark graphite field-console environment with a disciplined signal palette: cyan structures maps and navigation, yellow calls attention to command decisions, red marks critical incidents, and green communicates availability and confirmed state. Manrope keeps the app readable on small screens while DM Mono gives incident IDs, ETAs, and system labels an operational cadence.

The mobile layout is organized as a one-thumb command surface: compact top status, vertically stacked operational cards, high-contrast incident rows, and a fixed bottom navigation rail that becomes a side rail on wide screens. Motion is restrained and functional: short state changes, press feedback, and toast confirmations only. The entire experience remains clearly labeled as a simulation and product demonstration, not a certified live emergency system.
