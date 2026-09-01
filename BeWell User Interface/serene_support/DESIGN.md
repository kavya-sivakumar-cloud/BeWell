---
name: Serene Support
colors:
  surface: '#f8faf9'
  surface-dim: '#d8dada'
  surface-bright: '#f8faf9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f3'
  surface-container: '#eceeed'
  surface-container-high: '#e6e9e8'
  surface-container-highest: '#e1e3e2'
  on-surface: '#191c1c'
  on-surface-variant: '#3f484b'
  inverse-surface: '#2e3131'
  inverse-on-surface: '#eff1f0'
  outline: '#6f797c'
  outline-variant: '#bec8cb'
  surface-tint: '#086878'
  primary: '#006474'
  on-primary: '#ffffff'
  primary-container: '#2d7d8e'
  on-primary-container: '#f3fcff'
  inverse-primary: '#87d2e4'
  secondary: '#3c6569'
  on-secondary: '#ffffff'
  secondary-container: '#bce7ec'
  on-secondary-container: '#40696d'
  tertiary: '#894a0f'
  on-tertiary: '#ffffff'
  tertiary-container: '#a76227'
  on-tertiary-container: '#fff9f6'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#a9edff'
  primary-fixed-dim: '#87d2e4'
  on-primary-fixed: '#001f26'
  on-primary-fixed-variant: '#004e5b'
  secondary-fixed: '#bfeaee'
  secondary-fixed-dim: '#a4ced2'
  on-secondary-fixed: '#002022'
  on-secondary-fixed-variant: '#234d51'
  tertiary-fixed: '#ffdcc4'
  tertiary-fixed-dim: '#ffb780'
  on-tertiary-fixed: '#2f1400'
  on-tertiary-fixed-variant: '#6f3800'
  background: '#f8faf9'
  on-background: '#191c1c'
  surface-variant: '#e1e3e2'
  sos-red: '#D9534F'
  success-teal: '#4A9E91'
  surface-blue: '#E6F0F2'
  text-main: '#1A2E35'
typography:
  headline-lg:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 36px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 30px
  headline-md:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 26px
  body-md:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-sm:
    fontFamily: Atkinson Hyperlegible Next
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding: 20px
  stack-gap: 16px
  section-gap: 32px
---

## Brand & Style

The design system for this product is built on the principles of **calm, accessibility, and radical support**. Recognizing that users may be in states of high anxiety, low energy, or sensory overwhelm, the UI avoids all forms of visual "noise."

The chosen style is a blend of **Soft Minimalism and Glassmorphism**. We use generous whitespace to provide "breathing room" for the content, while utilizing subtle translucent layers to create a sense of depth without the harshness of heavy borders. The emotional goal is to evoke a "warm embrace"—a digital space that feels safe, non-judgmental, and profoundly easy to navigate. High contrast is maintained for legibility, but through soft color pairings rather than jarring black-on-white.

## Colors

The palette is rooted in **Soft Teals and Gentle Blues** to lower the heart rate and promote tranquility. 

- **Primary (#2D7D8E):** A deep, muted teal used for primary actions and brand presence. It provides enough contrast for accessibility while remaining "earthy."
- **Secondary (#8FB9BD):** A desaturated seafoam used for secondary buttons and supportive UI elements.
- **Tertiary (#F4A261):** A soft, warm sand tone used sparingly for "uplift" moments, such as completing a task or a positive mood check-in.
- **SOS Red (#D9534F):** A deliberate departure from the calm palette. This is a "safety red"—muted enough not to cause panic, but distinct enough to be found instantly in a crisis.
- **Neutral (#F8FAF9):** An off-white, mint-tinted background color to reduce eye strain compared to pure white.

## Typography

We have selected **Atkinson Hyperlegible Next** for the entire system. Developed specifically for high legibility, its distinctive character shapes help users with low vision or cognitive fatigue process information more easily.

- **Scale:** Headlines are bold but not massive, preventing an "aggressive" feel. 
- **Body Text:** Standardized at 18px for primary content to ensure effortless reading on mobile devices.
- **Line Height:** Tightened slightly for headlines but generous (1.5x) for body text to prevent "line skipping" during reading.

## Layout & Spacing

The layout follows a **Fluid Mobile-First** model. Given the nature of the app, the interface must never feel crowded.

- **Grid:** A simple 4-column grid for mobile, expanding to a centered max-width container on larger screens.
- **Rhythm:** An 8px base unit is used. Margins are intentionally wide (20px) to ensure touch targets for navigation (like the bottom bar) are easy to hit without error.
- **Reflow:** On desktop/tablet, the seven navigation tabs transition from a bottom bar to a fixed left-hand sidebar to maintain ergonomic access.

## Elevation & Depth

To maintain an "approachable" feel, we avoid harsh shadows and high-contrast borders.

- **Tonal Layering:** Depth is primarily communicated through color. Content sits on "Surface Blue" (#E6F0F2) cards against the "Neutral" background.
- **Soft Shadows:** When elevation is needed (e.g., the SOS button or active cards), use an ambient, highly diffused shadow: `box-shadow: 0 8px 24px rgba(45, 125, 142, 0.08)`. The shadow color is tinted with the primary teal to keep it feeling integrated rather than "dirty."
- **Backdrop Blur:** For modals and the bottom navigation, a `blur(10px)` effect is applied to provide context of the screen behind without visual distraction.

## Shapes

The design system uses a **Rounded** shape language to appear soft and non-threatening. 

- **Standard Elements:** Buttons and input fields use a 0.5rem (8px) radius.
- **Cards:** Larger containers (like those in the Activity dashboard or Peer Discovery) use `rounded-lg` (16px) to emphasize the "container" as a safe, enclosed space.
- **Interactive Pill:** Selection chips and the SOS button use a full pill shape to distinguish them as highly interactive elements.

## Components

### SOS Button
The most critical component. It is a floating action button (FAB), pill-shaped, using `sos-red`. It requires a "Press and Hold" (2 seconds) interaction, visualized by a circular progress border, to prevent accidental triggers while remaining accessible.

### Cards & Activity Dashboard
Activities are presented as large, rounded cards. Completed items desaturate and move to the bottom of the stack, using a subtle "Success Teal" checkmark. 

### Buttons
- **Primary:** Solid `primary-teal` with white text.
- **Secondary:** Ghost style with a `primary-teal` 2px border or solid `secondary-blue` for lower emphasis.
- **Touch Targets:** All buttons must have a minimum height of 48px for accessibility.

### Input Fields
Inputs use a soft `surface-blue` background instead of a white box to reduce "starkness." The active state is indicated by a 2px `primary-teal` border and a subtle glow.

### Chat & Anonymous Profiles
Peer profiles use generic avatars (geometric shapes or nature icons) and "Surface Blue" bubbles. This maintains the "anonymous but human" requirement. In the Chatbot tab, the AI’s messages are styled with a slight glassmorphism effect to distinguish them from human peers.