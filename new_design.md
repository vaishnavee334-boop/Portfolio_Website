# Vaishnavee Portfolio --- Design System

> **Purpose:** A practical visual and interaction specification for
> designing Vaishnavee's content-writing portfolio in Google Stitch and
> implementing it consistently across the website.
>
> **Creative direction:** Editorial magazine × personal literary
> journal. Sophisticated, curious, human, quietly playful, and
> unmistakably writer-led.
>
> **Reference:** [thatsallnikita.in](https://thatsallnikita.in/) --- use
> as aesthetic inspiration for the dark canvas, dusty-rose accents,
> expressive serif typography, personality-led details, and editorial
> layouts. Do not reproduce its exact compositions, copy, or identity.

------------------------------------------------------------------------

## 1. Design principles

1.  **Editorial first.** Typography, writing samples, and carefully
    composed layouts should carry the design---not decorative UI
    components.
2.  **Human, not corporate.** The site should feel like a thoughtful
    writer's personal corner of the internet, not an agency landing page
    or SaaS dashboard.
3.  **Expressive, but disciplined.** Use asymmetry, large headlines,
    annotations, and playful accents with a clear visual purpose.
4.  **Proof over claims.** Make room for real work, verified metrics,
    genuine testimonials, and publication links. Never invent
    credentials or results.
5.  **Readable by default.** Protect line length, contrast, hierarchy,
    and mobile readability even when layouts become expressive.
6.  **Consistent rhythm.** Reuse the same spacing scale, type scale,
    grid logic, colours, and interaction patterns throughout the site.

## 2. Colour palette

Use a restrained palette anchored by near-black, warm ivory, and dusty
rose. Pink is the signature accent; it should feel considered rather
than ubiquitous.

### Core tokens

  -----------------------------------------------------------------------
  Token                   Hex                     Intended use
  ----------------------- ----------------------- -----------------------
  `color-bg`              `#131315`               Main page background;
                                                  near-black charcoal

  `color-bg-raised`       `#1C1B1E`               Subtle raised surfaces,
                                                  menus, and alternate
                                                  dark sections

  `color-bg-soft`         `#242126`               Hover surfaces, chips,
                                                  and understated panels

  `color-text`            `#F7F0EB`               Primary text; warm
                                                  ivory rather than stark
                                                  white

  `color-text-muted`      `#C8BFC2`               Secondary copy,
                                                  metadata, captions

  `color-text-subtle`     `#9C9298`               Tertiary metadata only;
                                                  avoid for essential
                                                  information

  `color-accent`          `#B85D82`               Dusty rose; key words,
                                                  links, primary buttons

  `color-accent-hover`    `#CA7295`               Hover/focus state for
                                                  rose controls

  `color-accent-soft`     `#38232D`               Quiet pink-tinted
                                                  surface or selected
                                                  state

  `color-border`          `#393438`               Dividers, subtle
                                                  outlines, card edges

  `color-on-accent`       `#FFFFFF`               Text on rose buttons

  `color-on-light`        `#171518`               Text on light editorial
                                                  panels
  -----------------------------------------------------------------------

### Colour usage rules

-   Target roughly **75% dark canvas, 15% warm ivory, and 10% accent or
    supporting colour** across the full page. Treat this as a visual
    guide, not a strict pixel calculation.
-   Use `#131315` as the default canvas; avoid pure black because it can
    feel harsh.
-   Use warm ivory for headlines and primary copy. Reserve muted text
    for secondary information.
-   Use dusty rose to highlight selected words, active navigation,
    links, primary actions, and a few key statistics.
-   Do not make every heading pink. Contrast between ivory and rose is
    part of the identity.
-   Avoid introducing additional saturated colours or gradients. Any new
    colour must serve a clear content or accessibility purpose.
-   Light image backgrounds are acceptable inside portfolio screenshots
    or embedded work samples; frame them intentionally against the dark
    page.
-   Check contrast for all text sizes and interaction states. Do not
    rely on colour alone to communicate active, selected, or error
    states.

### Optional light editorial panel

A small number of work previews may use a warm paper-like panel for
contrast:

-   Panel: `#F7F0EB`
-   Main text: `#211C20`
-   Secondary text: `#625860`
-   Accent: `#A84970`

Use this sparingly. The website should remain predominantly dark.

## 3. Typography

### Recommended font pairing

**Display serif: `DM Serif Display`**\
Use for hero headlines, major section headings, pull quotes, selected
project titles, and expressive closing statements. It provides a
literary, magazine-like character without feeling overly formal.

**Body sans-serif: `DM Sans`**\
Use for paragraphs, navigation, buttons, labels, metadata, and longer
supporting copy. It is clean, contemporary, and readable.

**Optional handwritten accent:** Use a restrained handwritten font only
for one or two short annotations if the chosen font is legible. This is
optional---not a third core typeface. Never use it for body copy or
essential navigation.

If these fonts are unavailable in the design environment, use a
high-quality editorial serif such as `Cormorant Garamond` for display
and `Inter` for sans-serif text. Keep the pairing consistent throughout.

### Type scale

Use responsive sizes and adjust them to preserve the hierarchy at each
breakpoint.

  ---------------------------------------------------------------------------
  Style            Desktop size      Mobile size Weight /     Usage
                                                 line height  
  ------------ ---------------- ---------------- ------------ ---------------
  Display / H1        72--96 px        44--56 px Regular;     Hero statement
                                                 0.98--1.08   

  H2                  52--64 px        36--44 px Regular;     Major section
                                                 1.05--1.15   headings

  H3                  32--40 px        27--32 px Regular;     Service and
                                                 1.12--1.2    project titles

  H4                  23--28 px        21--24 px Medium or    Subsections
                                                 regular; 1.2 

  Lead                21--24 px        19--21 px Regular;     Hero and
                                                 1.45--1.6    section
                                                              introductions

  Body                16--18 px        16--17 px Regular;     Paragraphs
                                                 1.6--1.75    

  Small               14--15 px            14 px Regular;     Captions and
                                                 1.45--1.6    metadata

  Eyebrow             12--13 px            12 px Medium; 1.3  Category
                                                              labels,
                                                              uppercase
                                                              sparingly

  Button / nav        15--17 px        15--16 px Medium; 1.2  Actions and
                                                              navigation
  ---------------------------------------------------------------------------

### Typography rules

-   Keep display headlines mostly regular-weight; let size, contrast,
    line breaks, and spacing create impact.
-   Use sentence case for headings. Avoid unnecessary all-caps styling.
-   Use uppercase only for compact labels or category metadata, with
    subtle letter spacing of approximately `0.08em`.
-   Body text should generally have a measure of **55--75 characters per
    line** on desktop.
-   Keep paragraphs to a comfortable width---typically `55–68ch` for
    long-form reading.
-   Use a deliberate line break in the hero when it strengthens the
    message; avoid awkward orphan words.
-   Highlight one or two meaningful words in dusty rose when it adds
    emphasis. Do not colour entire paragraphs.
-   Use italics selectively for literary emphasis or short pull quotes.
-   Maintain a clear distinction between display serif and body
    sans-serif; do not switch typefaces arbitrarily between sections.

## 4. Spacing system

Use an 8 px base rhythm, with 4 px increments for fine adjustments.
Prefer consistent spacing tokens to one-off values.

  ------------------------------------------------------------------------
  Token                                        Value Typical use
  --------------------- ---------------------------- ---------------------
  `space-1`                                     4 px Tiny icon/text gap or
                                                     micro-adjustment

  `space-2`                                     8 px Tight inline spacing

  `space-3`                                    12 px Label and compact
                                                     control spacing

  `space-4`                                    16 px Standard element gap

  `space-5`                                    24 px Paragraph groups and
                                                     related controls

  `space-6`                                    32 px Card internals and
                                                     small layout gaps

  `space-7`                                    40 px Medium component
                                                     separation

  `space-8`                                    48 px Larger content group
                                                     spacing

  `space-9`                                    64 px Section subgroups

  `space-10`                                   80 px Compact section
                                                     padding

  `space-11`                                   96 px Standard section
                                                     padding

  `space-12`                                  120 px Spacious editorial
                                                     section padding

  `space-13`                                  144 px Occasional major
                                                     transition or hero
                                                     breathing room
  ------------------------------------------------------------------------

### Spacing rules

-   Desktop section padding: generally **96--128 px vertically**.
-   Tablet section padding: generally **72--96 px vertically**.
-   Mobile section padding: generally **56--72 px vertically**.
-   Keep related elements close and separate unrelated groups more
    generously.
-   Avoid excessive empty space that makes a section feel unfinished.
    Negative space must frame content, support hierarchy, or create a
    deliberate pause.
-   Use consistent gaps inside repeated grids and between repeated
    cards.
-   Avoid using different margins to force each section into place.
    Establish a shared grid and spacing logic instead.

## 5. Grid, alignment, and indentation

### Desktop grid

-   Use a centred content container with a maximum width of
    approximately **1240 px**.
-   At wide desktop widths, allow up to **1320 px** only when the layout
    benefits from the extra room.
-   Use a 12-column grid where useful, with consistent gutters of
    approximately **24 px**.
-   Maintain side margins of at least **48--64 px** on large screens.
-   Hero and editorial sections may be asymmetrical, but their elements
    should align to an underlying grid.
-   Do not force all sections into identical two- or three-column card
    layouts.

### Tablet grid

-   Use 8 columns where helpful.
-   Keep side margins around **32--40 px**.
-   Reduce grid gutters to **20--24 px**.
-   Collapse complex editorial compositions when their text or images
    become cramped.

### Mobile grid

-   Use a 4-column grid or a simple single-column flow.
-   Keep side padding around **20--24 px**.
-   Use **16 px** gaps for closely related items and **24--32 px**
    between distinct content groups.
-   Stack split layouts in a deliberate reading order: headline and
    context first, then supporting imagery or content where appropriate.
-   Prevent horizontal scrolling, clipped text, and tiny touch targets.

### Alignment and indentation rules

-   Align section headings, body copy, and primary content to a
    consistent section edge unless an intentional editorial offset is
    used.
-   Use indentation only to communicate hierarchy, such as a pull quote,
    supporting note, or nested detail.
-   Do not indent normal body paragraphs.
-   Keep bullet and list indentation consistent; align wrapped lines
    with the text rather than the bullet marker.
-   Align metadata and category labels consistently across project
    previews.
-   Decorative elements may extend beyond the content grid, but core
    text must remain readable and unclipped.
-   Use asymmetry deliberately---one offset image or headline is enough
    to create interest. Avoid random misalignment.

## 6. Section composition

### Header and navigation

-   Desktop header height: approximately **80--96 px**.
-   Keep the wordmark left-aligned and navigation right-aligned.
-   Use generous horizontal gaps without allowing the navigation to
    crowd the CTA.
-   Active navigation should use dusty rose and a subtle underline or
    another understated indicator.
-   Keep the header visually light; avoid a heavy bordered navigation
    bar.
-   On mobile, use a clear compact menu pattern with accessible
    controls.

### Hero

-   Aim for a visually memorable first viewport with a strong headline,
    short supporting copy, authentic portrait, and clear CTA.
-   Use a split or asymmetrical composition rather than a default
    centred hero.
-   Display headline width: approximately **8--11 words per visual line
    at most**, adjusted for the chosen copy and screen width.
-   Keep supporting copy narrow enough to scan.
-   Use no more than two primary actions in the hero.
-   A small eyebrow, annotation, or playful detail may add personality;
    keep it secondary to the message.
-   Make the hero feel complete at common laptop sizes without forcing
    all content above the fold.

### Content sections

-   Give each section a clear purpose and a recognisable visual rhythm.
-   Alternate between text-led sections, work previews, proof points,
    and more personal content to avoid repetitive scrolling.
-   Use pull quotes, dividers, image crops, and typography shifts to
    create transitions.
-   Avoid a card for every block of content. Use open layouts wherever a
    card adds no value.
-   Keep the selected-work section visually prominent; it is the
    strongest proof of writing ability.

### Footer and closing CTA

-   The closing CTA should feel like an editorial finale, with a large
    statement and one obvious next action.
-   The footer should be compact and functional, with readable contact
    information and social links.
-   Keep visual decoration restrained so the final action remains easy
    to find.

## 7. Buttons, links, and controls

### Primary button

-   Background: `#B85D82`
-   Text: `#FFFFFF`
-   Border radius: **999 px / pill**
-   Horizontal padding: **24--32 px**
-   Vertical padding: **14--18 px**
-   Text: `DM Sans`, 15--17 px, medium weight
-   Hover: move to `#CA7295` and apply a subtle transition
-   Focus: clear visible focus ring with adequate contrast

Use primary buttons for high-intent actions such as discussing a project
or contacting Vaishnavee.

### Secondary button

-   Prefer a transparent background with an ivory border or a simple
    text link with an arrow.
-   Use it for lower-priority actions such as exploring work or reading
    more.
-   Do not make every button visually equal.

### Text links

-   Use ivory by default and dusty rose for hover, active, or
    highlighted states.
-   Underline links where needed for clarity, especially inside
    paragraphs.
-   Give links a clear hover and keyboard-focus state.
-   External work samples should visibly behave like links and open the
    intended destination.

### Interaction sizing

-   Aim for touch targets of at least **44 × 44 px**.
-   Do not communicate clickability through colour alone.
-   Provide focus states for keyboard users.
-   Use transitions around **160--240 ms** with a restrained ease curve.

## 8. Cards, imagery, and project previews

### Project previews

-   Prefer editorial tiles with a title, category, short summary, and a
    clear link.
-   Allow selected projects to be larger than others to establish
    hierarchy.
-   Use consistent image ratios within a given group unless a deliberate
    feature layout calls for a different ratio.
-   Use subtle borders or background shifts only when needed to separate
    content.
-   Avoid generic icons in place of meaningful article titles, excerpts,
    or screenshots.

### Image treatment

-   Prioritise real portraits and genuine writing samples.
-   Use image crops that preserve the subject and support the
    composition.
-   Prefer understated square, portrait, or landscape crops according to
    content needs.
-   Avoid excessive filters, heavy overlays, and decorative frames
    around every image.
-   Use alt text for meaningful images; decorative imagery should not
    add redundant screen-reader content.
-   Keep placeholder assets visibly replaceable during development.

### Radius and borders

-   Use mostly square or subtly rounded corners for editorial imagery
    and content panels: **0--8 px**.
-   Pill radii are appropriate for buttons.
-   Do not turn every element into a rounded card.
-   Use `color-border` for fine dividers and occasional outlines rather
    than prominent boxes.

## 9. Decorative language

Use a small, consistent visual vocabulary:

-   Starburst or sparkle shapes used sparingly.
-   Short handwritten-style annotations, if legible.
-   Thin rules and underlines.
-   Oversized punctuation or isolated accent words.
-   Small category labels and editorial metadata.
-   Subtle offsets or overlap between imagery and text.

Rules:

-   Decorative elements should reinforce the page's rhythm or
    personality.
-   Keep decorations away from essential text and interactive controls.
-   Use one or two notable decorative moments per section at most.
-   Avoid confetti-like scatter, arbitrary floating shapes, excessive
    stickers, and ornamental elements that make the page feel cluttered.
-   Keep decorative shapes consistent in stroke, scale, and colour
    treatment.

## 10. Motion and interaction

Motion should feel calm, polished, and optional.

-   Use gentle opacity or vertical-reveal transitions for section
    entrances.
-   Add subtle image zoom or accent changes on hover where appropriate.
-   Use small underline animations for links.
-   Avoid aggressive parallax, bouncing elements, cursor-following
    effects, autoplaying media, and motion that delays access to
    content.
-   Do not animate every element independently.
-   Respect `prefers-reduced-motion` and provide a usable experience
    without animation.
-   Ensure interaction feedback is immediate and does not depend solely
    on animation.

## 11. Responsive breakpoints

Use these as starting points and adjust to content:

  ------------------------------------------------------------------------
  Breakpoint                                   Width Layout guidance
  --------------------- ---------------------------- ---------------------
  Mobile                                  `< 600 px` Single column,
                                                     compact navigation,
                                                     reduced display type

  Large mobile / small                  `600–767 px` Mostly stacked
  tablet                                             layout; introduce
                                                     limited two-column
                                                     groupings

  Tablet                               `768–1023 px` Flexible 8-column
                                                     grid; simplified
                                                     editorial offsets

  Desktop                             `1024–1439 px` Full editorial grid
                                                     and asymmetric
                                                     compositions

  Wide desktop                            `1440 px+` Constrain content
                                                     width; preserve
                                                     comfortable reading
                                                     measures
  ------------------------------------------------------------------------

### Responsive checks

-   Recompose rather than merely scale down.
-   Reduce decorative overlap on small screens.
-   Ensure all headings wrap naturally without clipping or isolated
    punctuation.
-   Stack service offerings and project previews in a readable order.
-   Keep body text at a comfortable mobile size.
-   Make buttons and navigation usable by touch.
-   Test long project titles, missing images, and lengthy excerpts.
-   Ensure the sticky or fixed header, if used, never covers section
    headings or anchor destinations.

## 12. Accessibility and content integrity

-   Maintain readable contrast, especially for muted text and
    rose-on-dark combinations.
-   Use semantic heading order: one primary H1, followed by logical H2
    and H3 sections.
-   Ensure every interactive element is keyboard accessible and visibly
    focused.
-   Use descriptive link labels rather than repeated "Click here."
-   Add meaningful alt text for content images.
-   Do not use colour as the sole way to indicate state.
-   Avoid text embedded in images when actual text can be used.
-   Use authentic, verified project details and testimonials only.
-   Label fictional demonstration content clearly and replace it before
    launch.
-   Do not invent rankings, traffic figures, client names, or
    professional claims.

## 13. Design tokens summary

Use the following as the default implementation tokens.

``` css
:root {
  /* Colours */
  --color-bg: #131315;
  --color-bg-raised: #1C1B1E;
  --color-bg-soft: #242126;
  --color-text: #F7F0EB;
  --color-text-muted: #C8BFC2;
  --color-text-subtle: #9C9298;
  --color-accent: #B85D82;
  --color-accent-hover: #CA7295;
  --color-accent-soft: #38232D;
  --color-border: #393438;
  --color-on-accent: #FFFFFF;
  --color-on-light: #171518;

  /* Typography */
  --font-display: "DM Serif Display", Georgia, serif;
  --font-body: "DM Sans", Arial, sans-serif;

  /* Content width */
  --content-max: 1240px;
  --content-max-wide: 1320px;
  --reading-max: 68ch;

  /* Spacing */
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-5: 24px;
  --space-6: 32px;
  --space-7: 40px;
  --space-8: 48px;
  --space-9: 64px;
  --space-10: 80px;
  --space-11: 96px;
  --space-12: 120px;

  /* Shape and motion */
  --radius-small: 4px;
  --radius-medium: 8px;
  --radius-pill: 999px;
  --transition-fast: 160ms ease;
  --transition-standard: 220ms ease;
}
```

## 14. Final quality checklist

Before approving the design, confirm that:

-   [ ] The visual identity consistently uses charcoal, warm ivory, and
    dusty rose.
-   [ ] Serif display typography and sans-serif body typography have
    distinct, consistent roles.
-   [ ] The page feels editorial and personal rather than corporate or
    template-driven.
-   [ ] Spacing follows a consistent rhythm and the layout aligns to a
    shared grid.
-   [ ] Negative space feels intentional and no section feels empty or
    unfinished.
-   [ ] The hero immediately communicates Vaishnavee's value and
    personality.
-   [ ] Selected work is easy to browse and gives writing the visual
    priority.
-   [ ] Credibility claims are grounded in the supplied information.
-   [ ] Placeholder content is easy to identify and replace.
-   [ ] Buttons, links, and navigation have hover, focus, and responsive
    states.
-   [ ] Mobile layouts have been deliberately recomposed and remain
    readable.
-   [ ] Motion is subtle, accessible, and never blocks content.
-   [ ] Every section contributes to the same coherent brand story.

**North star:** Make the website feel like stepping into the mind of a
curious, thoughtful writer---an editorial space with taste, warmth,
clarity, and enough personality to be memorable.
