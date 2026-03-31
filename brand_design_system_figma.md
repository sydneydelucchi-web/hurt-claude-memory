# HURT! Brand Design System — Extracted from Figma

> Figma file URLs and active feedback status: see `memory/reference_figma.md`

---

## Typography

### Headings — Urbanist
| Level | Size | Line Height |
|-------|------|-------------|
| H1 | 64px | 68px |
| H2 | 54px | 60px |
| H3 | 42px | 48px |
| H4 | 34px | 38px |
| H5 | 26px | 30px |
| H6 | 22px | 28px |

### Body / Paragraphs — Inter
| Level | Size | Line Height |
|-------|------|-------------|
| P20 | 25px | 28px |
| P18 | 18px | 22px |
| P16 | 16px | 24px |
| P14 | 14px | 22px |
| P13 | 13px | 20px |

### Mobile Headings — Urbanist
| Level | Size | Line Height |
|-------|------|-------------|
| H1 | 40px | 36px |
| H2 | 36px | 36px |
| H3 | 32px | 36px |
| H4 | 28px | 36px |
| H5 | 24px | 28px |
| H6 | 22px | 28px |

### Font Import
- Google Fonts: `Urbanist:wght@400;500;600;700;800` and `Inter:wght@400;500;600;700`

---

## Color Palette

### Primary Colors (HURT! Red Spectrum)
| Name | Hex | Usage |
|------|-----|-------|
| Black | #000000 | Text, darkest UI |
| HURT! Deep Red | #BE281A | Primary brand red, logo |
| HURT! Red | #BF3422 | Buttons, CTAs |
| HURT! Coral | #DC4E33 | Accent, hover states |
| Warm Coral | #E5B150 | Warm accent |
| Salmon | #F69E93 | Light accent |
| Blush | #FBC2B8 | Card backgrounds |
| Light Pink | #FFF1F0 | Section backgrounds |
| Pale Blush | #FEF8FA | Hero/section backgrounds |
| Alert/Brand Yellow | #9F3422 | Deep accent variant |

### Neutrals
| Hex | Usage |
|-----|-------|
| #FAFAFA | Lightest background |
| #F2F2F2 | Card/section background |
| #EAEBEB | Borders, dividers |
| #EEEEE9 | Subtle background |
| #D3D4D5 | Disabled states |
| #B1B3E4 | Light accent (lavender tint) |
| #979958 | Muted accent |
| #737878 | Secondary text |
| #4B4741 | Dark text alt |
| #123384 | Deep blue accent |
| #191B1A | Near-black text |

### Secondary Colors — Teal/Green (Used in Solutions Hub, HDR)
| Name | Hex | Usage |
|------|-----|-------|
| Dark Teal | #0C667E | HDR primary, section backgrounds |
| Teal | #31A6B2 | HDR accents, CTAs |
| Green-Teal | #38A893 | HDR success states |
| Mid Teal | #59BEC9 | HDR progress elements |
| Employer/Solutions Teal | (dark teal CTA sections) | Solutions Hub employer pages |

### Secondary Colors — Lavender
| Name | Hex | Usage |
|------|-----|-------|
| Lavender 800 | #201D4F | Deep purple |
| Lavender 700 | #3B83FB | (needs verification) |
| Lavender 500 | #6383FB | Mid lavender |
| Lavender 300 | #A1A1F3 | Light lavender |
| Lavender 100 | #E5E0DC | Pale lavender |
| Lavender 50 | #FDF0FF | Lightest lavender |

### Gradients
- Coral-to-teal blended gradients
- Soft pink-to-white fades for hero backgrounds
- Multi-stop gradients with brand reds and teals

---

## Visual Language

### Shape Language
- **Rounded corners**: Pill-shaped buttons, rounded cards (border-radius: 8-16px typical)
- **HURT! "X" motif**: Crossed pattern used as decorative/brand texture element
- **Circular elements**: Progress rings (HDR), avatar frames, icon containers

### Illustration Style
- **Website**: Flat, colorful character illustrations — friendly, diverse, simplified
- **HDR Product**: Purple/lavender character figures with teal accents — exercise/fitness poses, more detailed than website icons
- **Icon style**: Clean line icons for navigation; filled rounded icons for features

### Photography
- Real photography used alongside illustrations
- Exercise/rehab photography in HDR Activity View
- Stock photography for Solutions Hub sections (real patients, real settings)

### Device Mockups
- MacBook laptop + iPhone combo mockup for hero sections
- Red phone frame for mobile app screenshots
- Always shown at slight angle for dimensionality

---

## UI Components

### Buttons
| Type | Style |
|------|-------|
| Primary CTA | Red/coral pill button (#BF3422 bg, white text, full rounded) |
| Secondary CTA | Outlined pill button (border only, text link style) |
| HDR Primary | Dark teal pill button (#0C667E bg, white text) |
| Text Link | "Already a Partner? Login →" with arrow |

### Navigation
- **Website**: Full-width top nav, matches hero background color, transitions to white with 1px grey stroke on scroll
- **Menu items**: Platform, Solutions, Resources, Company, For Patients
- **Right side**: Sign In → | Book a Demo (red pill)
- **HDR Desktop**: "HURT! Digital Rehab" header with Home / Settings / Log Out

### Cards
- Rounded corners, subtle shadows
- Feature cards with icon + title + description
- Exercise cards with photo thumbnail + title + duration
- Metric cards with large stat number + label

### Sections
- Hero: Pink/salmon background (#FEF8FA) with device mockup
- Social proof: "Trusted by experts/Trusted by Forward-Thinking Employers" with partner logos
- Feature grid: 2-3 column card layouts
- Stats bar: Sliding metric module (4.5★ / 24/7 / <2min)
- Dark teal CTA section: Full-width dark background with conversion content
- FAQ: Accordion-style expandable
- Footer: Dark background, multi-column

---

## Page Templates (Website)

### Homepage
- Hero with tagline + device mockup + dual CTA
- Social proof bar (partner logos)
- "Built to Elevate the Orthopedic Experience" feature cards
- "One Integrated Platform. Complete MSK Care" section
- Testimonials/case studies
- CTA section
- Footer

### Solutions Hub (3 Variants)
- **Orthopedic Practices**: Red/coral primary theme
- **For Employers**: Teal/green primary theme
- **For Digital Rehab**: Teal/green primary theme
- All follow same modular structure:
  1. Hero with headline + illustration/mockup
  2. Social proof bar
  3. Feature image/photography section
  4. Value proposition with icon cards
  5. Metrics section ("The Return on Modern MSK Access")
  6. Product showcase
  7. Performance stats (sliding metric module: 4.5★ / 24/7 / <2min)
  8. Dark teal CTA section
  9. FAQ
  10. Bottom CTA

### Platform Overview
- Main overview page
- Sub-pages: SuperDash, Joint Score, ATC, HURT! Pass, 24/7 Triage
- Modular section-based layouts

---

## HDR Product UI

### Desktop Views
- **Care Plan View**: Left sidebar (Today / My Care Plan) + main content with progress ring (60% complete), character illustrations, checklist
- **Activity View**: Exercise cards with real photography, video/audio/activity icons, "Start Exercise" teal CTA
- **Frame width**: 1,200px

### Mobile Views
- Dark teal header with body map interaction
- Exercise screens with character illustrations
- Activity lists with tab navigation
- Bottom navigation bar

### HDR Color Tokens (from layers)
- #0C667E (primary dark teal)
- #59BEC9 (mid teal / progress)
- #38A893 (green-teal / success)
- #31A6B2 (teal / accent)
- #868686 (gray / inactive)
- #BABABA (light gray / disabled)

### HDR Isolated Assets
- Character exercise illustrations (extractable)
- Icon sets (active/inactive states)
- UI component library elements

---

## Design System Components (from Figma)
The Figma Design System page contains these documented frames:
1. Brand (Foundation)
2. Colours
3. Typography
4. Grid System (Desktop + Mobile + Spacers)
5. Logos
6. Icons
7. Stock Photos
8. Visuals (HURT! X motif patterns)
9. Components
10. Buttons
11. Tags, Eyebrows & Pagination
12. Input Fields
13. Modules
14. Footer

> Active design feedback and Figma file URLs: see `memory/reference_figma.md`
