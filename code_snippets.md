# Code Snippets: Landing Page Project

This document extracts and documents selective, reusable code snippets from the Landing Page project, focusing on HTML structures and CSS properties, particularly Flexbox. All items are new compared to previous notes from the Odin Recipes project, which covered basic HTML5 structure, colors, fonts, and simple layouts without Flexbox or advanced semantic elements.

## HTML Snippets

### Navigation Structure

```html
<div class="nav">
  <div class="logo">Motivation Central</div>
  <ul class="links">
    <li><a href="">Home</a></li>
    <li><a href="">Speakers</a></li>
    <li><a href="">Events</a></li>
    <li><a href="">Contact</a></li>
  </ul>
</div>
```

- **Key Concept**: Semantic navigation with logo and unordered list for links.

### Card Layout Structure

```html
<div class="cards">
  <div class="card">
    <div class="card-image-wrapper">
      <img src="./images/shia.jpg" alt="" class="info-image" />
    </div>
    <p class="info-text">
      Shia LaBeouf's "Just Do It!" inspires action and determination.
    </p>
  </div>
  <!-- More cards -->
</div>
```

- **Key Concept**: Reusable card components with image wrapper and text for content sections.

### Quote with Figure Element

```html
<figure>
  <blockquote class="quote">
    Don't aim at success. The more you aim at it and make it a target, the more
    you are going to miss it...
  </blockquote>
  <figcaption>-Viktor E. Frankl</figcaption>
</figure>
```

- **Key Concept**: Semantic figure element for quotes with blockquote and figcaption.

### Call-to-Action Section

```html
<div class="action-wrapper">
  <div class="action-items">
    <div class="action-text-wrapper">
      <h3 class="action-title">Join the Motivation Movement!</h3>
      <p class="action-text">
        Sign up for exclusive content, event updates, and motivational tips from
        our speakers, and more!
      </p>
    </div>
    <button class="btn action-btn">Sign up</button>
  </div>
</div>
```

- **Key Concept**: Action-oriented sections with text and button for user engagement.

## CSS Snippets

### Flexbox Navigation

```css
.nav {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  margin-bottom: 110px;
}
```

- **Key Concept**: Flexbox for horizontal layout with space distribution and baseline alignment.

### Flexbox Content Layout

```css
.content {
  display: flex;
  align-items: center;
  gap: 50px;
}

.text-container,
.image-wrapper {
  flex: 1;
}
```

- **Key Concept**: Flexbox for side-by-side content with equal flex distribution and gap spacing.

### Flexbox Card Grid

```css
.cards {
  display: flex;
  justify-content: center;
  gap: 50px;
}
```

- **Key Concept**: Flexbox for horizontal card arrangement with centering and gaps.

### Flexbox Action Items

```css
.action-items {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
}
```

- **Key Concept**: Flexbox for distributing action text and button with space-between and center alignment.

### Flexbox Footer

```css
.copyright {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
}
```

- **Key Concept**: Flexbox for centering copyright text with icon.

### Image Object Fit

```css
.info-image {
  object-fit: cover;
  max-width: 140%;
  object-position: -28px 0;
}
```

- **Key Concept**: Object-fit for responsive image cropping and positioning.

### Button Styling

```css
.btn {
  padding: 6px 36px;
  border-radius: 9px;
  background-color: #3882f6;
  color: #f9faf8;
  font-weight: 900;
  font-size: 18px;
}

.action-btn {
  min-width: 140px;
  border: 3px solid #f9faf8;
}
```

- **Key Concept**: Reusable button styles with variants for different actions.

## Notes on New Items

- **Flexbox Properties**: Extensive use of `display: flex`, `justify-content` (space-between, center), `align-items` (baseline, center), `gap`, and `flex: 1` for responsive layouts not present in previous notes.
- **Semantic HTML Elements**: Introduction of `nav`, `figure`, `blockquote`, `figcaption` for better structure and accessibility.
- **Advanced CSS**: Properties like `object-fit`, `object-position`, `overflow`, `border-radius`, and `letter-spacing` for enhanced styling.
- **Layout Concepts**: Multi-section page structure with class-based sections (section-1 to section-5) for modular design.
- **No JavaScript**: Consistent with previous notes, no JS functions identified.
