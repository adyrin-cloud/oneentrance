# OneEntrance - UX & Branding Specification

**Inspired by:** North End Coffee Roasters  
**Created:** March 16, 2026  
**Version:** 1.0

---

## 1. Brand Identity

### Brand Essence
- **Tagline Inspiration:** "sourcing, roasting, and brewing specialty coffee since 2011"
- **Core Values:** Quality, Craftsmanship, Community, Premium Experience
- **Tone of Voice:** Warm, Professional, Approachable, Authentic
- **Brand Personality:** Sophisticated yet welcoming, artisanal, detail-oriented

---

## 2. Color Palette

### Primary Colors
```css
--primary-dark-brown: #2C1810;      /* Deep espresso brown - main headers */
--primary-coffee: #5C4033;          /* Rich coffee brown - primary actions */
--primary-cream: #F4EDE4;           /* Warm cream - backgrounds */
--primary-gold: #C8A882;            /* Golden latte - accents */
```

### Secondary Colors
```css
--secondary-mocha: #8B6F47;         /* Mocha - secondary elements */
--secondary-beige: #E8DCC8;         /* Light beige - cards, sections */
--secondary-charcoal: #4A4A4A;      /* Charcoal - body text */
--secondary-warm-gray: #6D5D52;     /* Warm gray - subtle text */
```

### Accent Colors
```css
--accent-green: #3D5A3C;            /* Coffee plant green - success states */
--accent-terracotta: #C17855;       /* Warm terracotta - highlights */
--accent-copper: #B87333;           /* Copper - premium features */
```

### Neutral Colors
```css
--neutral-white: #FFFFFF;           /* Pure white */
--neutral-off-white: #FAF8F5;       /* Off-white - main background */
--neutral-light-gray: #E5E5E5;      /* Light gray - borders */
--neutral-medium-gray: #999999;     /* Medium gray - disabled states */
--neutral-dark: #1A1A1A;            /* Almost black - contrast text */
```

### Semantic Colors
```css
--success: #3D5A3C;                 /* Green - success messages */
--error: #A84432;                   /* Muted red - error states */
--warning: #D4A574;                 /* Warm amber - warnings */
--info: #5C7A8B;                    /* Cool blue-gray - info */
```

---

## 3. Typography

### Font Families
```css
/* Primary Heading Font */
--font-heading: 'Playfair Display', 'Georgia', serif;
/* Alternative: 'Merriweather', 'Lora', 'Crimson Text' */

/* Body & UI Font */
--font-body: 'Inter', 'Helvetica Neue', Arial, sans-serif;
/* Alternative: 'Open Sans', 'Lato', 'Source Sans Pro' */

/* Monospace (for data/code) */
--font-mono: 'JetBrains Mono', 'Courier New', monospace;
```

### Font Scales
```css
/* Headings */
--font-size-h1: 3.5rem;      /* 56px - Hero headlines */
--font-size-h2: 2.5rem;      /* 40px - Section headers */
--font-size-h3: 2rem;        /* 32px - Subsections */
--font-size-h4: 1.5rem;      /* 24px - Card titles */
--font-size-h5: 1.25rem;     /* 20px - Small headers */
--font-size-h6: 1.125rem;    /* 18px - Micro headers */

/* Body Text */
--font-size-base: 1rem;      /* 16px - Base body text */
--font-size-large: 1.125rem; /* 18px - Large body text */
--font-size-small: 0.875rem; /* 14px - Small text */
--font-size-tiny: 0.75rem;   /* 12px - Captions, labels */

/* Line Heights */
--line-height-tight: 1.2;
--line-height-normal: 1.5;
--line-height-relaxed: 1.75;
--line-height-loose: 2;

/* Font Weights */
--font-weight-light: 300;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
```

---

## 4. Spacing System

### Base Unit: 8px
```css
--space-xs: 0.5rem;    /* 8px */
--space-sm: 1rem;      /* 16px */
--space-md: 1.5rem;    /* 24px */
--space-lg: 2rem;      /* 32px */
--space-xl: 3rem;      /* 48px */
--space-2xl: 4rem;     /* 64px */
--space-3xl: 6rem;     /* 96px */
--space-4xl: 8rem;     /* 128px */
```

### Container Widths
```css
--container-xs: 480px;
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1536px;
```

---

## 5. UI Components

### Border Radius
```css
--radius-sm: 4px;      /* Small elements */
--radius-md: 8px;      /* Cards, buttons */
--radius-lg: 12px;     /* Large cards */
--radius-xl: 16px;     /* Hero sections */
--radius-full: 9999px; /* Circular elements */
```

### Shadows
```css
--shadow-sm: 0 1px 2px rgba(44, 24, 16, 0.05);
--shadow-md: 0 4px 6px rgba(44, 24, 16, 0.07);
--shadow-lg: 0 10px 15px rgba(44, 24, 16, 0.1);
--shadow-xl: 0 20px 25px rgba(44, 24, 16, 0.15);
--shadow-2xl: 0 25px 50px rgba(44, 24, 16, 0.25);

/* Coffee-themed glow */
--shadow-warm: 0 8px 16px rgba(200, 168, 130, 0.3);
```

### Buttons
```css
/* Primary Button */
.btn-primary {
  background: var(--primary-coffee);
  color: var(--neutral-white);
  padding: 12px 24px;
  border-radius: var(--radius-md);
  font-weight: var(--font-weight-semibold);
  box-shadow: var(--shadow-md);
  transition: all 0.3s ease;
}

.btn-primary:hover {
  background: var(--primary-dark-brown);
  box-shadow: var(--shadow-lg);
  transform: translateY(-2px);
}

/* Secondary Button */
.btn-secondary {
  background: transparent;
  color: var(--primary-coffee);
  border: 2px solid var(--primary-coffee);
  padding: 12px 24px;
  border-radius: var(--radius-md);
}

/* Tertiary/Ghost Button */
.btn-ghost {
  background: transparent;
  color: var(--primary-coffee);
  padding: 12px 24px;
  text-decoration: underline;
  text-underline-offset: 4px;
}
```

### Cards
```css
.card {
  background: var(--neutral-white);
  border-radius: var(--radius-lg);
  padding: var(--space-lg);
  box-shadow: var(--shadow-md);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: var(--shadow-xl);
}

.card-image {
  width: 100%;
  height: 240px;
  object-fit: cover;
  border-radius: var(--radius-md);
}
```

### Navigation
```css
.navbar {
  background: var(--neutral-white);
  backdrop-filter: blur(10px);
  box-shadow: var(--shadow-sm);
  padding: var(--space-sm) 0;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.nav-link {
  color: var(--secondary-charcoal);
  font-weight: var(--font-weight-medium);
  text-transform: uppercase;
  letter-spacing: 0.05em;
  font-size: var(--font-size-small);
  transition: color 0.3s ease;
}

.nav-link:hover,
.nav-link.active {
  color: var(--primary-coffee);
}
```

---

## 6. Layout Patterns

### Hero Section
```
- Full-width background image (coffee/roasting/cafe atmosphere)
- Overlay with subtle gradient (dark to transparent)
- Centered heading + tagline
- Primary CTA button
- Minimum height: 70vh
- Text alignment: Center
```

### Cafe Listing Grid
```
- Responsive grid: 1 col (mobile) → 2 cols (tablet) → 3 cols (desktop)
- Card-based design with image + content
- Image aspect ratio: 4:3
- Includes: Location name, area, brief description
- Hover effect: Lift + enhanced shadow
```

### Section Layout
```
- Alternating image + text sections
- Generous whitespace between sections (var(--space-3xl))
- Section headers centered with decorative element
- Max-width for readability: 1280px
```

---

## 7. Imagery Guidelines

### Photo Style
- **Type:** High-quality, professional photography
- **Subjects:** Coffee preparation, cafe interiors, beans, latte art, ambiance
- **Tone:** Warm, inviting, natural light
- **Filter:** Slight warm tone boost, rich contrast
- **Avoid:** Over-processed, artificial lighting, stock photos

### Image Specifications
```
Hero Images: 1920x1080px (16:9)
Cafe Cards: 800x600px (4:3)
Gallery: 800x800px (1:1)
Logo/Icons: SVG format preferred
```

### Icon Style
- **Type:** Line icons (2px stroke weight)
- **Style:** Minimalist, rounded corners
- **Color:** Inherit from context or var(--primary-coffee)
- **Library Suggestion:** Heroicons, Feather Icons, Lucide

---

## 8. Animation & Transitions

### Timing Functions
```css
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-smooth: cubic-bezier(0.25, 0.1, 0.25, 1);
```

### Durations
```css
--duration-fast: 150ms;
--duration-normal: 300ms;
--duration-slow: 500ms;
```

### Common Animations
```css
/* Fade In */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* Slide Up */
@keyframes slideUp {
  from { transform: translateY(20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

/* Hover Lift */
.interactive:hover {
  transform: translateY(-4px);
  transition: transform var(--duration-normal) var(--ease-out);
}
```

---

## 9. Responsive Breakpoints

```css
/* Mobile First Approach */
--breakpoint-xs: 480px;   /* Small phones */
--breakpoint-sm: 640px;   /* Large phones */
--breakpoint-md: 768px;   /* Tablets */
--breakpoint-lg: 1024px;  /* Small laptops */
--breakpoint-xl: 1280px;  /* Desktops */
--breakpoint-2xl: 1536px; /* Large screens */
```

### Grid System
```css
/* Mobile: 4 columns, 16px gutters */
/* Tablet: 8 columns, 24px gutters */
/* Desktop: 12 columns, 32px gutters */
```

---

## 10. User Experience Patterns

### Navigation Structure
```
Home
├── About
├── Our Cafes
│   └── Individual Cafe Details
├── Coffee Journey
│   ├── Sourcing
│   ├── Roasting
│   └── Brewing
├── Menu (if applicable)
└── Contact
```

### Cafe Card Interaction
1. **Default State:** Card with image, title, location
2. **Hover:** Lift effect, show "View Details" overlay
3. **Click:** Navigate to individual cafe page or open modal
4. **Mobile:** Tap to expand inline details

### Loading States
- **Skeleton screens** for content loading
- **Progress bars** for multi-step processes
- **Spinners** for quick actions
- Use coffee brown color for loaders

### Empty States
- Friendly messaging (e.g., "No cafes found nearby")
- Illustration or icon
- Clear call-to-action to resolve

---

## 11. Accessibility (a11y)

### Color Contrast
- **Level AA Compliance:** Minimum 4.5:1 for normal text
- **Level AAA Target:** 7:1 for enhanced readability
- Verify all color combinations with contrast checker

### Focus States
```css
*:focus-visible {
  outline: 2px solid var(--primary-coffee);
  outline-offset: 2px;
  border-radius: var(--radius-sm);
}
```

### ARIA & Semantic HTML
- Use semantic HTML5 elements (`<nav>`, `<main>`, `<article>`)
- Provide alt text for all images
- ARIA labels for interactive elements
- Keyboard navigation support

### Text Sizing
- Minimum font size: 14px
- Allow text scaling up to 200%
- Use relative units (rem, em)

---

## 12. Content Guidelines

### Headings
- **H1:** Page title, one per page
- **H2:** Major sections
- **H3:** Subsections
- Use sentence case for headings
- Keep concise (5-10 words)

### Body Copy
- Short paragraphs (3-4 sentences)
- Bullet points for lists
- Active voice
- Line length: 60-80 characters for optimal readability

### Microcopy
- Buttons: Action-oriented (e.g., "Find Your Cafe", "Explore Locations")
- Errors: Helpful, non-technical
- Success: Positive, encouraging

---

## 13. Special Features (North End Inspired)

### Coffee Journey Section
- 3-step visual journey: Bean → Roastery → Cup
- Use high-quality process photos
- Animated scroll reveal
- Informative tooltips

### Location Finder
- Interactive map integration (Google Maps)
- Filter by area/neighborhood
- "Nearest to me" geolocation feature
- Distance display

### Social Integration
- Instagram feed grid (3x3 or responsive)
- Live updates from social media
- Hashtag display: Brand hashtag
- Social share buttons

### Newsletter/Updates
- Simple email capture form
- Minimal fields (email only)
- Positioned in footer or as modal
- Privacy-conscious messaging

---

## 14. PWA-Specific Enhancements

### App Icon
- Coffee cup or logo-based icon
- Warm brown color scheme
- Sizes: 192x192, 512x512
- Maskable icon support

### Splash Screen
- Brand logo centered
- Background: var(--primary-cream)
- Loading indicator: Coffee brown

### Offline Experience
- Cached cafe listings
- "You're offline" message with coffee cup illustration
- Show previously viewed cafes
- Queue actions for when back online

### Install Prompt
- Custom install prompt after user engagement
- Benefit-focused messaging
- Respect user dismissal

---

## 15. Implementation Checklist

### Phase 1: Foundation
- [ ] Setup CSS custom properties (colors, spacing, typography)
- [ ] Implement base typography styles
- [ ] Create component library (buttons, cards, inputs)
- [ ] Setup responsive grid system

### Phase 2: Core Pages
- [ ] Hero section with imagery
- [ ] Cafe listing grid
- [ ] Individual cafe detail view
- [ ] Navigation component

### Phase 3: Features
- [ ] Map integration
- [ ] Image gallery/carousel
- [ ] Social media integration
- [ ] Contact form

### Phase 4: Polish
- [ ] Animations and transitions
- [ ] Loading states
- [ ] Error handling
- [ ] Accessibility audit
- [ ] Performance optimization

---

## 16. Design Resources

### Fonts
- **Playfair Display:** [Google Fonts](https://fonts.google.com/specimen/Playfair+Display)
- **Inter:** [Google Fonts](https://fonts.google.com/specimen/Inter)

### Icon Libraries
- Heroicons: https://heroicons.com/
- Feather Icons: https://feathericons.com/
- Lucide: https://lucide.dev/

### Stock Photos (Coffee-themed)
- Unsplash: Coffee collection
- Pexels: Cafe/coffee search
- Actual product photography (preferred)

### Color Tools
- Coolors.co: Palette generator
- Contrast Checker: WebAIM
- Adobe Color: Harmony testing

---

## 17. Brand Voice Examples

### Primary Messaging
✅ "Your neighborhood coffee retreat"  
✅ "Crafted with passion, served with care"  
✅ "From bean to cup, excellence in every step"  

### Call-to-Actions
✅ "Find Your Nearest Cafe"  
✅ "Explore Our Locations"  
✅ "Start Your Coffee Journey"  
✅ "Visit Us Today"  

### Avoid
❌ "Click here"  
❌ "Submit"  
❌ Generic corporate speak  
❌ Overly casual/slang  

---

**Last Updated:** March 16, 2026  
**Maintained By:** Development Team  
**Review Cycle:** Quarterly
