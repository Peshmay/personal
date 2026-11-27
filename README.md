# Patience Evertsson Portfolio Website

## Project Overview

The project demonstrates semantic HTML, responsive CSS, accessibility, CSS Grid, Flexbox, reusable design tokens, and responsive.

## Key Features

### Portfolio Content

- Home and Hero introduction
- About section
- Experience and Education timelines
- Six project cards
- My work
- Footer with copyright information

## Responsive Design

- Desktop, tablet, and mobile layouts
- Three-, two-, and one-column project grids
- Stacked content on smaller screens
- Responsive images and typography
- CSS-only hamburger navigation
- No horizontal scrolling

## Accessibility

- Semantic HTML landmarks
- Logical heading structure
- Descriptive image alternatives
- Form labels connected to their fields
- Visible keyboard focus indicators
- Readable colour contrast
- Reduced-motion support
- Keyboard-operable navigation

## Website Structure

The website follows a semantic one-page structure:

- <header> contains the logo, navigation, contact link, and mobile menu.
- <main> contains the primary website content.
- <section> separates the Home, About, Experience, Projects, Gallery, and Contact content.
- <article> represents each independent project card.
- <figure> and <figcaption> group gallery images with captions.
- <form> contains the contact fields.
- <footer> contains the copyright information.

## Main Sections

## Header and Navigation

The sticky header remains visible while the visitor scrolls. At widths of 850px and below, the mobile navigation changes into a CSS-only hamburger menu.

## Hero

The desktop Hero uses a split background, an arched portrait, and an overlapping information card. On mobile, the portrait becomes circular and appears above the text.

## About

The About section combines a tall arched portrait with a text card. The image and text sit beside each other on desktop and stack vertically on smaller screens.

## Experience and Education

Education and employment are displayed in two timeline cards. The cards change to a single-column layout on smaller screens.

## Projects

Six project cards are displayed in a responsive grid:

- Desktop: three columns
- Tablet: two columns
- Mobile: one column

## Gallery

The Gallery uses semantic <figure> and <figcaption> elements. Its grid changes from three columns to two columns and then one column as the screen becomes smaller.

## My work

- Display my work assignments

## Design System

The visual identity combines deep plum headings, warm cream surfaces, muted body text, and a controlled gold accent.
:root {
--plum: #42184f;
--gold: #bd9140;
--dark: #211c23;
--text: #715878;
--cream: #fffdf9;
--light-cream: #faf7f1;
--blush: #f4eaf0;
--border: #e8dfd4;
}

## Typography

- Headings: Cormorant Garamond
- Body, navigation, buttons, and forms

## Spacing

The layout follows an 8px-based spacing approach. Responsive clamp() values control large headings and horizontal spacing without requiring many extra breakpoints.

## Seed Constraint

My seed constraint is the gold accent colour #BD9140. I used it consistently for emphasis, active navigation, important labels, borders, timeline markers, and hover feedback. I avoided using it as the dominant background colour, so it guides attention without overwhelming the design.
The seed can be identified in several parts of the website:

- Navigation hover and active states
- Introductory labels
- Highlighted heading text
- Timeline dots and connecting lines
- Card borders and decorative details
- Button and link feedback

## Technologies

## Core

- HTML5
- CSS3
- CSS Grid
- Flexbox
- CSS custom properties
- CSS media queries

## Assets

- Google Fonts
- Font Awesome icons

## Project Constraint

- No JavaScript

## Responsive Behaviour

The website uses media queries to adapt its navigation, columns, images, typography, and spacing. The main mobile breakpoint is 850px, with an additional small-phone breakpoint at 520px.
Anchor targets use scroll-margin-top so section headings are not hidden behind the sticky header.

## Problems Solved

1. The Contact Me button was missing from the open mobile menu.
2. Anchor links positioned headings incorrectly below the sticky header.
3. The Contact form was too tall and required unnecessary scrolling.
4. The About portrait needed a better shape and stronger balance with its text card.
5. Decorative project numbers, lines, and circles made the design too busy.
6. An old padding-top rule pushed the Contact introduction below the form.
7. These issues were solved by correcting selectors, removing conflicting declarations, refining spacing, improving image sizing, adding suitable media queries, and simplifying unnecessary decoration.

## Testing

1. The website’s HTML was checked using the W3C Markup Validation Service. Document checking completed with no errors or warnings

2. The website’s CSS was checked using the W3C CSS Validator at CSS Level 3 + SVG, and no errors were found.

3. The website was visually checked at desktop, tablet, and mobile widths. Testing covered:

- Header and navigation behaviour
- Hamburger menu operation
- Anchor-link positions
- Project and gallery grids
- Image scaling and cropping
- Contact form alignment
- Alternative text and form labels
- Keyboard focus indicators
- Reduced-motion rules
- Horizontal overflow
- The screenshots in the build log provide evidence of the layout at different development stages and screen sizes.
# personal
