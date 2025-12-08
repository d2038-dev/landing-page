# Flexbox Code Snippets from Odin Project Landing Page

This document extracts high-quality, reusable flexbox examples from the Odin Project landing page project (`/home/d2038-dev/repos/top/landing-page`). Snippets focus on advanced flexbox concepts like containers, axis control, alignment, and item sizing, demonstrating best practices for responsive layouts in headers, hero sections, content areas, and footers. Each snippet includes context, explanation, and reference to the original CSS.

## Flex Containers and Basic Setup

### Navigation Header with Space Distribution

```css
.nav {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 110px;
}
```

**Context**: Used in the header section (`.section-1`) to create a horizontal navigation bar with logo on the left and links on the right.  
**Explanation**: `display: flex` establishes the flex container. `justify-content: space-between` distributes items along the main axis with maximum space between them. `align-items: baseline` aligns items to their text baselines for consistent vertical positioning. This pattern is ideal for headers requiring left/right alignment without equal spacing.  
**Reference**: `style.css:32-37`

### Horizontal Link List

```css
.links {
  list-style: none;
  padding: 0;
  display: flex;
  gap: 26px;
  letter-spacing: 0.4px;
}
```

**Context**: Applied to the navigation links in the header.  
**Explanation**: `display: flex` on the `<ul>` creates a flex container for list items. `gap: 26px` provides consistent spacing between flex items, replacing margins. This demonstrates flexbox for inline navigation menus.  
**Reference**: `style.css:56-62`

## Main/Cross Axis Control and Alignment

### Hero Section with Centered Vertical Alignment

```css
.content {
  display: flex;
  align-items: center;
  gap: 50px;
}
```

**Context**: Layouts the hero content in `.section-1`, placing text and image side by side.  
**Explanation**: `align-items: center` centers items along the cross axis (vertically in row direction). `gap: 50px` ensures spacing. This pattern is common for hero sections needing balanced vertical alignment.  
**Reference**: `style.css:70-74`

### Call-to-Action Section with Space Distribution

```css
.action-items {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
}
```

**Context**: Used in the action section (`.section-4`) for text and button layout.  
**Explanation**: `justify-content: space-between` pushes items to opposite ends of the main axis. `align-items: center` centers them vertically. `gap: 30px` adds minimum spacing. Effective for sections with text on one side and actions on the other.  
**Reference**: `style.css:175-180`

### Footer Copyright Centering

```css
.copyright {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
}
```

**Context**: Centers the copyright text in the footer (`.section-5`).  
**Explanation**: `justify-content: center` centers items along the main axis. `align-items: center` centers vertically. This is a standard pattern for footer content alignment.  
**Reference**: `style.css:207-212`

## Item Sizing and Equal Distribution

### Equal Flex Sizing for Hero Elements

```css
.text-container,
.image-wrapper {
  flex: 1;
}
```

**Context**: Applied to text and image containers in the hero section.  
**Explanation**: `flex: 1` (shorthand for `flex-grow: 1; flex-shrink: 1; flex-basis: 0`) makes items equally distribute available space. This ensures responsive equal-width columns in hero layouts.  
**Reference**: `style.css:76-79`

## Content Area Layouts

### Centered Card Grid

```css
.cards {
  display: flex;
  justify-content: center;
  gap: 50px;
}
```

**Context**: Arranges speaker cards in `.section-2`.  
**Explanation**: `justify-content: center` centers the flex items as a group. `gap: 50px` spaces them evenly. This pattern works well for centered content grids without wrapping (assuming fixed item widths).  
**Reference**: `style.css:114-118`
