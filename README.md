# Zero JS Carousel

A zero-dependency, responsive image slider built exclusively with HTML markup and standard CSS styling rules. 

## Overview & Value Proposition

Modern web development leans heavily on JavaScript packages for basic UI components. This often adds unnecessary build steps, bundle bloat, and maintenance overhead. 

`Zero JS Carousel` demonstrates how far native browser standards can take you. By leveraging hidden HTML radio inputs paired with CSS sibling combinations (`~`), this project provides full pagination, next/previous navigation controls, and visual thumbnail indicators without writing a single line of JavaScript.

## How It Works

The mechanics rely on standard DOM input states:

1. **State Storage:** A set of radio buttons with matching `name` attributes store the current active slide index.
2. **Conditional Rendering:** CSS selector chains target `:checked` inputs to translate the slide wrapper container along the X-axis.
3. **Control Binding:** HTML `<label>` elements use the `for` attribute to switch checked states when clicked, acting as trigger targets for pagination and navigation arrows.

## Key Features

* Zero JavaScript runtime dependency.
* Hardware-accelerated transitions via CSS `transform`.
* Dynamic next/previous directional arrows linked to slide state.
* Visual indicator dots for direct slide selection.
* Clean separation of structure and presentation.

## Tech Stack Breakdown

* **HTML5:** Semantic structure, form input primitives, structural labels.
* **CSS3:** Flexbox layouts, relative positioning, state-driven selectors (`:checked`, `~`).

## Prerequisites & Web-Based Quick Start

You don't need Node.js, npm, or local terminal tooling to inspect or run this repository.

### Option 1: GitHub Codespaces (In-Browser)

1. Press `.` on your keyboard while viewing this repository, or click the **Code** button and select **Open with Codespaces**.
2. Once the editor loads, open `index.html`.
3. Right-click inside the file editor and choose **Preview HTML** or use an extension like Live Preview to render the page directly inside the browser.

### Option 2: Local Setup

1. Download or clone the files (`index.html` and `style.css`).
2. Double-click `index.html` to open it in any modern web browser.

## Repository Structure

```text
zero-js-carousel/
├── .github/
│   └── workflows/
│       └── html-lint.yml    # Validates HTML structure on push
├── .gitignore               # Excludes OS and editor junk files
├── index.html               # Main markup structure with state inputs[cite: 1]
├── style.css                # Layout styles and state transitions[cite: 1]
├── LICENSE                  # MIT License details
└── README.md                # Project documentation
```

## Roadmap

[ ] Add smooth keyboard navigation support using HTML tab indices.

[ ] Implement dark mode styling using CSS custom properties.

[ ] Add touch swipe gestures using CSS scroll snap mechanics.
