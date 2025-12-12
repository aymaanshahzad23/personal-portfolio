# Personal Portfolio Design Guidelines

## Design Approach
**Reference-Based Minimal Portfolio Style** - Drawing inspiration from modern developer portfolios (Vercel, Linear, Rauno's portfolio) with emphasis on typography hierarchy, generous whitespace, and functional elegance.

## Core Design Principles
1. **Whitespace First** - Content breathes with generous margins and padding
2. **Typography Hierarchy** - Clear distinction between heading levels and body text
3. **Functional Minimalism** - Every element serves a purpose
4. **Dark Mode Parity** - Equal quality in both light and dark modes

## Typography System
- **Headings**: Inter or SF Pro Display
  - H1 (Hero): text-5xl md:text-7xl, font-bold, tracking-tight
  - H2 (Section): text-3xl md:text-4xl, font-bold
  - H3 (Subsection): text-xl md:text-2xl, font-semibold
- **Body**: Inter or SF Pro Text
  - Primary: text-base md:text-lg, leading-relaxed
  - Secondary: text-sm md:text-base, opacity-70
- **Metrics/Numbers**: Tabular numerals, font-mono for technical details

## Layout & Spacing System
**Spacing Units**: Use Tailwind units of 4, 8, 12, 16, 20, 24 (p-4, m-8, gap-12, py-16, etc.)

**Container Strategy**:
- Max-width: max-w-6xl for main content
- Hero: max-w-4xl for centered text
- Sections: py-20 md:py-32 for vertical rhythm
- Inner spacing: px-6 md:px-8

**Grid System**:
- Projects: grid-cols-1 md:grid-cols-2 gap-8
- Skills: grid-cols-2 md:grid-cols-4 gap-4
- Experience: Single column with timeline decoration

## Component Specifications

### Hero Section (No Background Image)
- Text-only centered layout with generous top padding (pt-32 md:pt-48)
- Name as H1 with gradient text effect on accent color
- Professional title as large body text
- Brief tagline (1-2 sentences)
- CTA buttons: "View Projects" + "Contact Me" in horizontal layout
- Social links (GitHub, LinkedIn, Email) as icon row below CTAs
- Scroll indicator at bottom (subtle down arrow)

### About Section
- Two-column layout on desktop: Professional photo (rounded-2xl, w-64 h-64) + bio text
- Mobile: Stack photo above text
- Bio: 2-3 paragraphs with key achievements and specializations
- Stats row: Years of experience, Projects completed, Technologies mastered (if metrics available)

### Experience Timeline
- Vertical timeline with connecting line (border-l-2 on container)
- Each entry: Company logo circle + company name + role + dates + bullet achievements
- Achievements as metric-driven bullet points (3-5 per role)
- Timeline dots: Absolute positioned circles at -left-1

### Project Cards
- Hover-lift effect (translate-y-1 shadow transition)
- Structure: Project image/icon + Title + Description + Tech stack tags + Metrics/results + Links
- Tech stack: Inline badge pills with small padding
- Links: "View Project" + "GitHub" (if available) as subtle text links
- Card spacing: p-6, rounded-xl, border subtle

### Skills Section
- Category-grouped badges (Frontend, Backend, Tools, etc.)
- Badge style: Pill shape (rounded-full px-4 py-2), centered text
- Grid with responsive columns
- Hover state: Slight scale effect

### Education Section
- Clean card layout: Institution + Degree + Dates + Achievements/GPA
- If multiple degrees: Vertical stack with spacing

### Contact Section
- Form on left (2/3 width), contact info on right (1/3 width) on desktop
- Mobile: Stack form above info
- Form fields: Name, Email, Message (textarea)
- Field style: Border-b-2 only (minimal underline style), no background
- Submit button: Full width on mobile, inline on desktop
- Contact info: Email, LinkedIn, GitHub with icons
- No map or additional visual elements needed

### Dark Mode Toggle
- Fixed position top-right corner (top-8 right-8)
- Icon button (sun/moon) with smooth rotation transition
- Persistent via localStorage
- Ensure all text maintains readability in both modes

## Navigation
- Sticky header with logo/name on left, nav links on right
- Mobile: Hamburger menu with slide-in overlay
- Nav links: Smooth scroll to sections
- Minimal border-b separator

## Animations
- **Page load**: Stagger fade-in for hero elements only
- **Scroll reveals**: Subtle fade-up for section headers (intersection observer)
- **Hover states**: Transform scale-105 for cards, underline for links
- **NO scroll-driven parallax or excessive motion**

## Responsive Breakpoints
- Mobile: Base (< 768px) - Single column, stacked layouts
- Tablet: md (768px+) - Two columns where appropriate
- Desktop: lg (1024px+) - Full multi-column layouts

## Images
**Hero**: No background image - text-only minimal design
**About**: Professional headshot (square format, 256x256px minimum)
**Projects**: Optional project preview images (16:9 ratio) - if not available, use placeholder with project icon/logo

This design creates a sophisticated, content-focused portfolio that emphasizes professional achievements while maintaining visual clarity and modern aesthetics.