Gruvbox Dark Hard Theme: Color Palette & SCSS Usage Guide

Gruvbox is a popular retro-groove color scheme designed to be easy on the eyes, with sufficient contrast and pleasant, muted (yet distinct) colors. The "Dark Hard" variant uses a very dark background for higher contrast compared to the standard or soft dark versions.

This guide provides the color palette for Gruvbox Dark Hard and suggestions for their application, especially when using SCSS for a website.
Core Palette Philosophy

    Backgrounds: Dark, desaturated tones providing a comfortable base.

    Foregrounds: Lighter, warm, desaturated tones for text and primary content.

    Accents: A set of distinct, muted and brighter retro colors (red, green, yellow, blue, aqua, purple, orange) used for highlighting, status indicators, and UI elements.

SCSS Variable Naming Convention

We'll use a consistent naming convention for SCSS variables:
$gruvbox-[type]-[name]-[variant]
Example: $gruvbox-bg-hard, $gruvbox-fg-primary, $gruvbox-red-strong, $gruvbox-grey-medium
I. Background Colors

These are the foundational colors for your site's backdrop.

    Primary Background (Hard Contrast)

        SCSS: $gruvbox-bg-hard: #1d2021;

        Usage: The main, darkest background for the entire page or large content areas. This is the defining color of the "hard" contrast variant.

    Slightly Lighter Background / UI Elements

        SCSS: $gruvbox-bg-medium: #282828;

        Usage: Can be used for secondary background areas, cards, sidebars, or elements that need to be distinct from the primary hard background but still dark. (This is the standard Gruvbox dark background).

    Subtle Background Variations / Borders

        SCSS: $gruvbox-bg-soft: #32302f;

        Usage: For subtle layering, inactive UI elements, or borders that need to be darker than content but lighter than the main background.

    Darker Grey Tones (for depth, dividers, or hover states)

        SCSS: $gruvbox-bg1: #3c3836;

        SCSS: $gruvbox-bg2: #504945;

        SCSS: $gruvbox-bg3: #665c54;

        SCSS: $gruvbox-bg4: #7c6f64;

        Usage:

            $gruvbox-bg1: For elements like modal headers, footers, or slightly elevated panels.

            $gruvbox-bg2: For hover states on dark elements, input field backgrounds.

            $gruvbox-bg3: For subtle dividers, borders on interactive elements.

            $gruvbox-bg4: Can act as a very dark foreground or a lighter background for specific components needing less contrast with text.

II. Foreground Colors

These colors are primarily for text and icons.

    Primary Foreground (Main Text)

        SCSS: $gruvbox-fg-primary: #fbf1c7;

        Usage: The main color for body text, headings, and general content against the dark backgrounds.

    Brighter Foreground / Emphasized Text

        SCSS: $gruvbox-fg-bright: #ebdbb2;

        Usage: For headings, important labels, or active navigation items that need to stand out slightly more than primary text.

    Muted Foreground / Secondary Text

        SCSS: $gruvbox-fg-muted: #d5c4a1;

        Usage: For secondary text, helper text, captions, or disabled text.

    Dimmer Foreground / Tertiary Text

        SCSS: $gruvbox-fg-dim: #bdae93;

        Usage: For less important information, placeholder text, or very subtle annotations.

    Darkest Foreground / Very Muted Text

        SCSS: $gruvbox-fg-dark: #a89984;

        Usage: For subtle text on slightly lighter dark backgrounds (e.g., on $gruvbox-bg2 or $gruvbox-bg3), or for elements that should recede.

III. Accent Colors

Gruvbox features a set of vibrant (strong) and more subdued (muted) accent colors.
1. Red

    Strong Red

        SCSS: $gruvbox-red-strong: #fb4934;

        Usage: Errors, destructive actions (e.g., delete buttons), critical alerts, danger indicators.

    Muted Red

        SCSS: $gruvbox-red-muted: #cc241d;

        Usage: Less critical warnings, error message text (if strong red is too harsh for blocks of text), icons for errors.

2. Green

    Strong Green

        SCSS: $gruvbox-green-strong: #b8bb26;

        Usage: Success messages, confirmations, positive actions (e.g., save buttons), validation success.

    Muted Green

        SCSS: $gruvbox-green-muted: #98971a;

        Usage: Subtle success indicators, icons for completed tasks, less prominent positive feedback.

3. Yellow

    Strong Yellow

        SCSS: $gruvbox-yellow-strong: #fabd2f;

        Usage: Warnings, attention-grabbing notifications (non-critical), highlighting important information or pending states.

    Muted Yellow

        SCSS: $gruvbox-yellow-muted: #d79921;

        Usage: Less urgent warnings, informational callouts, icons for alerts.

4. Blue

    Strong Blue

        SCSS: $gruvbox-blue-strong: #83a598;

        Usage: Primary actions (e.g., main call-to-action buttons), links, informational icons, active states for navigation or tabs. Often used for interactive elements.

    Muted Blue

        SCSS: $gruvbox-blue-muted: #458588;

        Usage: Secondary links, less prominent informational elements, borders for focused elements, subtle highlights.

5. Purple (Magenta)

    Strong Purple

        SCSS: $gruvbox-purple-strong: #d3869b;

        Usage: Special status indicators, tags, categories, or for adding a distinct visual flair to certain UI elements. Can be used for user-generated content tags or specific event types.

    Muted Purple

        SCSS: $gruvbox-purple-muted: #b16286;

        Usage: Less prominent tags, secondary status text, or decorative elements where a subtle touch of purple is desired.

6. Aqua

    Strong Aqua

        SCSS: $gruvbox-aqua-strong: #8ec07c;

        Usage: Often used for strings or special constants in code highlighting. In a website, it can be an alternative to blue for links or informational callouts, providing a slightly different feel. Good for highlighting specific data points or features.

    Muted Aqua

        SCSS: $gruvbox-aqua-muted: #689d6a;

        Usage: Subtle highlights, decorative elements, or text that needs to be distinct but not as prominent as strong aqua. Can be used for blockquotes or code snippets.

7. Orange

    Strong Orange

        SCSS: $gruvbox-orange-strong: #fe8019;

        Usage: Secondary warnings, attention-grabbing elements that aren't errors (e.g., "beta" tags, important announcements), or as a vibrant accent for specific UI components.

    Muted Orange

        SCSS: $gruvbox-orange-muted: #d65d0e;

        Usage: Less critical alerts, icons for pending actions, or as a more subdued warm accent.

IV. Neutral Grey Tones

These are derived from the background/foreground ramp and are useful for UI chrome, borders, and subtle distinctions.

    Darkest Grey (Main Background)

        SCSS: $gruvbox-grey-darkest: #1d2021; (Same as $gruvbox-bg-hard)

    Dark Grey

        SCSS: $gruvbox-grey-dark: #282828; (Same as $gruvbox-bg-medium)

    Medium-Dark Grey

        SCSS: $gruvbox-grey-medium-dark: #3c3836; (Same as $gruvbox-bg1)

    Medium Grey

        SCSS: $gruvbox-grey-medium: #504945; (Same as $gruvbox-bg2)

    Light-Medium Grey

        SCSS: $gruvbox-grey-light-medium: #665c54; (Same as $gruvbox-bg3)

    Light Grey (can be a muted foreground)

        SCSS: $gruvbox-grey-light: #7c6f64; (Same as $gruvbox-bg4)

    Very Light Grey / Darkest Foreground

        SCSS: $gruvbox-grey-lighter: #928374;

        Usage: Often a muted background in some Gruvbox variants, or a very dim foreground/icon color.

    Off-White / Muted Foreground

        SCSS: $gruvbox-grey-off-white: #a89984; (Same as $gruvbox-fg-dark)

V. Implementing with SCSS

When implementing this in SCSS, define these variables at the top of your main stylesheet or in a dedicated _variables.scss file.

// _variables.scss

// Backgrounds
$gruvbox-bg-hard: #1d2021;
$gruvbox-bg-medium: #282828;
$gruvbox-bg-soft: #32302f;
$gruvbox-bg1: #3c3836;
$gruvbox-bg2: #504945;
$gruvbox-bg3: #665c54;
$gruvbox-bg4: #7c6f64;

// Foregrounds
$gruvbox-fg-primary: #fbf1c7;
$gruvbox-fg-bright: #ebdbb2;
$gruvbox-fg-muted: #d5c4a1;
$gruvbox-fg-dim: #bdae93;
$gruvbox-fg-dark: #a89984;

// Accent Colors - Strong
$gruvbox-red-strong: #fb4934;
$gruvbox-green-strong: #b8bb26;
$gruvbox-yellow-strong: #fabd2f;
$gruvbox-blue-strong: #83a598;
$gruvbox-purple-strong: #d3869b;
$gruvbox-aqua-strong: #8ec07c;
$gruvbox-orange-strong: #fe8019;

// Accent Colors - Muted
$gruvbox-red-muted: #cc241d;
$gruvbox-green-muted: #98971a;
$gruvbox-yellow-muted: #d79921;
$gruvbox-blue-muted: #458588;
$gruvbox-purple-muted: #b16286;
$gruvbox-aqua-muted: #689d6a;
$gruvbox-orange-muted: #d65d0e;

// Neutral Greys (some are aliases)
$gruvbox-grey-darkest: $gruvbox-bg-hard;
$gruvbox-grey-dark: $gruvbox-bg-medium;
$gruvbox-grey-medium-dark: $gruvbox-bg1;
$gruvbox-grey-medium: $gruvbox-bg2;
$gruvbox-grey-light-medium: $gruvbox-bg3;
$gruvbox-grey-light: $gruvbox-bg4;
$gruvbox-grey-lighter: #928374;
$gruvbox-grey-off-white: $gruvbox-fg-dark;

// --- Example Usage ---
// body {
//   background-color: $gruvbox-bg-hard;
//   color: $gruvbox-fg-primary;
// }

// a {
//   color: $gruvbox-blue-strong;
//   &:hover {
//     color: $gruvbox-aqua-strong;
//   }
// }

// .button-primary {
//   background-color: $gruvbox-blue-muted;
//   color: $gruvbox-fg-primary;
// }

// .alert-error {
//   background-color: $gruvbox-red-muted;
//   color: $gruvbox-fg-bright;
//   border-left: 3px solid $gruvbox-red-strong;
// }

This comprehensive list should give you a solid foundation for theming your website with Gruvbox Dark Hard. Remember to test for accessibility (WCAG contrast ratios) when combining these colors, especially for text against various backgrounds.