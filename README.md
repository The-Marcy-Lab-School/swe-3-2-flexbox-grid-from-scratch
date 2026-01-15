# Checkpoint 3 - HTML & CSS (Music Player)

- [Overview](#overview)
- [Setup](#setup)
- [Design Specifications](#design-specifications)
  - [Guiding Questions \& Suggestions](#guiding-questions--suggestions)
  - [Style Guide](#style-guide)
  - [Additional Styling Notes](#additional-styling-notes)
- [CSS Cheatsheet](#css-cheatsheet)
  - [Colors](#colors)
  - [Typography (Text Styling)](#typography-text-styling)
  - [Box Model (Spacing \& Sizing)](#box-model-spacing--sizing)
  - [Layout](#layout)
  - [Interactive States (Pseudo-classes)](#interactive-states-pseudo-classes)
  - [Flexbox](#flexbox)
  - [Grid](#grid)
  - [Media Queries](#media-queries)
- [Submission](#submission)

## Overview

In this assignment, you will be building and styling a **Spotify-style Music Player page** using HTML, Flexbox, Grid from scratch using nothing more than a design document to reference!

Use the previous assignment to see the patterns for how to structure your page and how to use flexbox/grid to style the page.

**What's Provided:**
- Empty HTML file (`index.html`)
- CSS reset (`style.css`)

**Your Task:**
- Build the entire HTML content and structure
- Write CSS to match the design specifications
- Use CSS Grid and Flexbox for the appropriate sections

## Setup

1. Open the `src/index.html` file in your browser and set up the boilerplate (type `html:5` and hit enter)
2. Write your HTML in `src/index.html` and CSS in `src/style.css`
3. Refresh the browser frequently to see your changes

**Tips:**
- Use your browser's Developer Tools (right-click > Inspect) to debug CSS issues
- Resize your browser window to test responsive behavior
- If a style isn't working, check for typos and missing semicolons!

## Design Specifications

Use the spec diagram below and the following style guide to build your page.

![Specifications for mobile and desktop views](./img/spec.png)

### Guiding Questions & Suggestions

Before you start coding, take a moment to analyze the design:

**HTML Structure:**
- What are the main sections of this page? How can you use semantic elements (`header`, `main`, `footer`, `section`, `nav`) to structure your HTML?
- What repeating patterns do you see? Use lists (`ul`, `li`) to represent them.

**Layout Strategy:**
- Where do you see elements arranged in a single row or column? These are good candidates for **Flexbox**.
- Where do you see elements arranged in a two-dimensional grid pattern (rows AND columns)? These are good candidates for **CSS Grid**.


### Style Guide

Use the following fonts and colors for this project:

- Font family: `'Segoe UI', Tahoma, Geneva, Verdana, sans-serif`
- Text color: `#ffffff` (pure white)
- Accent green text color: `#1db954`
- Black background color: `#000000` (pure black)
- Dark grey background color: `#1e1e1e`

### Additional Styling Notes

- Remove text decoration (underlines) from nav links
- Links should turn green on hover

## CSS Cheatsheet

Use this as a reference while working. **You don't need to memorize these!**

Here is a reference of the CSS properties we've learned. **You don't need to memorize these!** Use this as a reference while working.

### Colors

| Property                           | What It Does          | Example                |
| ---------------------------------- | --------------------- | ---------------------- |
| `color`                            | Sets text color       | `color: midnightblue;` |
| `background` or `background-color` | Sets background color | `background: azure;`   |

Color values can be: named colors (`red`, `blue`), hex codes (`#FF5733`), or RGB (`rgb(255, 87, 51)`).

### Typography (Text Styling)

| Property          | What It Does                | Example                           |
| ----------------- | --------------------------- | --------------------------------- |
| `font-family`     | Sets the font               | `font-family: Arial, sans-serif;` |
| `font-size`       | Sets text size (use `rem`!) | `font-size: 1.5rem;`              |
| `font-weight`     | Sets boldness               | `font-weight: bold;`              |
| `font-style`      | Sets italic                 | `font-style: italic;`             |
| `text-align`      | Aligns text                 | `text-align: center;`             |
| `text-decoration` | Adds/removes underlines     | `text-decoration: none;`          |

### Box Model (Spacing & Sizing)

| Property                                                     | What It Does                 | Example                           |
| ------------------------------------------------------------ | ---------------------------- | --------------------------------- |
| `width`                                                      | Sets element width           | `width: 300px;`                   |
| `max-width`                                                  | Sets maximum width           | `max-width: 600px;`               |
| `padding`                                                    | Space INSIDE the border      | `padding: 20px;`                  |
| `margin`                                                     | Space OUTSIDE the border     | `margin: 10px;`                   |
| `border`                                                     | Creates a border (all sides) | `border: 2px solid black;`        |
| `border-top`, `border-bottom`, `border-left`, `border-right` | Border on one side           | `border-bottom: 2px solid black;` |
| `border-radius`                                              | Rounds corners               | `border-radius: 8px;`             |

**Shorthand for padding/margin:**
- `padding: 10px;` → all sides
- `padding: 10px 20px;` → top/bottom, left/right

### Layout

| Property       | What It Does                             | Example             |
| -------------- | ---------------------------------------- | ------------------- |
| `margin: auto` | Centers a block element (needs a width!) | `margin: auto;`     |
| `list-style`   | Styles/removes list bullets              | `list-style: none;` |

### Interactive States (Pseudo-classes)

```css
/* When mouse hovers over element */
a:hover {
  background: lightblue;
}
```

### Flexbox

| Property          | What It Does                              | Example                          |
| ----------------- | ----------------------------------------- | -------------------------------- |
| `display: flex`   | Makes the element a flex container        | `display: flex;`                 |
| `flex-direction`  | Sets direction: `row` (default), `column` | `flex-direction: column;`        |
| `justify-content` | Spacing along the **main axis**           | `justify-content: space-between` |
| `align-items`     | Alignment along the **cross axis**        | `align-items: center;`           |
| `gap`             | Space **between** flex items              | `gap: 20px;`                     |

**Common `justify-content` values:** `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, `space-evenly`

**Common `align-items` values:** `flex-start`, `flex-end`, `center`, `stretch` (default)

### Grid

| Property                | What It Does                     | Example                             |
| ----------------------- | -------------------------------- | ----------------------------------- |
| `display: grid`         | Makes the element a grid         | `display: grid;`                    |
| `grid-template-columns` | Defines column sizes             | `grid-template-columns: 1fr 1fr;`   |
| `gap`                   | Space between grid items         | `gap: 20px;`                        |

**The `fr` unit** divides available space into fractions. `1fr 1fr 1fr` creates 3 equal columns.

### Media Queries

```css
/* Styles for screens 600px and wider */
@media (min-width: 600px) {
  .selector {
    /* styles here */
  }
}
```

---

## Submission

When you are finished:
1. Save all your files
2. Commit your changes with a descriptive message
3. Push to your repository
4. Make a pull request and tag your instructors for review
5. Submit the link to your pull request
