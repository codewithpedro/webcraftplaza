### The Project Planning & Execution Framework

This framework breaks down the development process into three distinct stages:

1.  **The Blueprint Phase:** A pre-code planning stage to define the project.
2.  **The Plan Document:** A structured to-do list that is easy to read and edit.
3.  **The Phased Execution:** A step-by-step implementation of the plan.

---

### Stage 1: The Blueprint Phase (Before You Code)

Before creating any files or writing code, answer these questions to create a clear blueprint.

#### 1. Project Definition
*   **Main Goal:** What is the single most important goal of this project? (e.g., *To build a portfolio website to attract freelance clients.*)
*   **Key Features:** List the non-negotiable features. (e.g., *About Me section, a filterable gallery of my work, a working contact form.*)
*   **Target Audience:** Who will be using this? (e.g., *Tech recruiters, potential clients, other developers.*)

#### 2. Information & Content
*   **Sitemap:** Map out all the pages and how they connect.
    *   *Example: Home -> About, Home -> Projects -> Project Detail, Home -> Contact.*
*   **Content Inventory:** List all the text, images, and data you will need.
    *   *Example: Bio text, project descriptions, screenshots for each project, resume PDF.*

#### 3. Design & User Experience (UX)
*   **Inspiration:** Gather 2-3 examples of websites you like. What do you like about them?
*   **Wireframe:** Create a simple, low-fidelity sketch for each page. Focus only on the layout and placement of elements. This is crucial for planning your HTML structure. **You can even draw this on paper.**

⚠️ **Note:** Before moving on to the next stage. Let me check the checklist to see if I want to add or edit anything. 

---

### Stage 2: Create The `PLAN.md` Document

Now, convert the blueprint into a structured to-do list. Create a new file named `PLAN.md` in your project's root directory. Use the template below to organize your tasks. The use of Markdown checklists (`- [ ]`) allows you to track progress visually.

Use the template below to organize your tasks. The use of Markdown checklists (`- [ ]`) allows you to track progress visually.

⚠️ **Note:** Before moving on to the next phase, you must test the current work and confirm it meets expectations. After completing a phase, **ask the project owner (me) to review and approve**. Only after I say “continue,” may you proceed to the next phase.


#### `PLAN.md` Template

```markdown
# Project Plan: [Your Project Name]

**Goal:** [Copy from Blueprint Phase]

---

## Phase 1: Project Setup & Tooling

- [ ] Create project folder structure (`/assets`, `/css-styles`, `/js-tools`)
- [ ] Use Tailwind via CDN (`<script src="https://cdn.tailwindcss.com"></script>`)
- [ ] Create initial files: `index.html`, `css-styles/main.css`, `js-tools/app.js`
- [ ] (Optional) Add inline Tailwind config in `<script>` tag for theme customization


---

## Phase 2: HTML Scaffolding (Structure First)

*Goal: Build the semantic HTML structure for all pages based on the wireframes. Do not add any styling yet.*

- [ ] **Homepage:**
    - [ ] Create `<header>` with navigation
    - [ ] Create `<main>` content area
    - [ ] Add hero section
    - [ ] Add project highlights section
    - [ ] Create `<footer>`
- [ ] **About Page:**
    - [ ] Create header and footer
    - [ ] Add bio section
- [ ] **Projects Page:**
    - [ ] Create header and footer
    - [ ] Add project gallery grid
- [ ] **Contact Page:**
    - [ ] Create header and footer
    - [ ] Build the HTML for the contact form (`<form>`, `<label>`, `<input>`)

---

## Phase 3: Styling (Mobile-First with Tailwind CSS)

*Goal: Apply styles to the existing HTML structure. Start with mobile views, then add responsive styles for larger screens.*

- [ ] **Global Styles:**
    - [ ] Define fonts and base colors in `tailwind.config.js`
- [ ] **Components:**
    - [ ] Style the navigation bar
    - [ ] Style the buttons
    - [ ] Style the footer
- [ ] **Pages:**
    - [ ] Style the Homepage (mobile & desktop)
    - [ ] Style the About Page (mobile & desktop)
    - [ ] Style the Projects Page (mobile & desktop)
    - [ ] Style the Contact Page (mobile & desktop)
- [ ] **Animations:**
    - [ ] Add fluid and minimal animations using Tailwind’s built-in classes (e.g., `transition`, `duration-300`, `ease-in-out`)
    - [ ] Use animations to subtly enhance elements like buttons, cards, and page transitions


---

## Phase 4: JavaScript & Interactivity

*Goal: Add functionality to the styled components.*

- [ ] Implement mobile menu toggle button
- [ ] Add validation for the contact form
- [ ] (If applicable) Fetch project data from an API and display it
- [ ] Add any hover effects or small animations

---

## Phase 5: Finalization & Optimization

- [ ] **Review:**
    - [ ] Proofread all content for typos
    - [ ] Test the site on different browsers (Chrome, Firefox, Safari)
    - [ ] Test the site on a real mobile device
- [ ] **Optimization:**
    - [ ] Compress all images in the `assets` folder
    - [ ] Minify CSS and JavaScript for production
    - [ ] Run an accessibility audit (e.g., Lighthouse) and fix issues
- [ ] **Deployment:**
    - [ ] Deploy the final code to the web host

```

---

### Stage 3: Phased Execution

With your `PLAN.md` file ready, you can now start coding.

1.  **Work Through One Phase at a Time:** Start with "Phase 1: Project Setup". Do not move to Phase 2 until all items in Phase 1 are checked off.
2.  **Focus on the Goal of Each Phase:**
    *   When you are in the HTML phase, **ignore styling**.
    *   When you are in the CSS phase, **avoid changing the HTML structure**.
3.  **Update the Plan:** As you complete each task, mark the checkbox (`- [x]`). This provides a clear sense of progress and keeps you on track.
4.  **Edit the Plan as Needed:** A plan is a guide, not a rigid set of rules. If you discover a new requirement or realize a task is unnecessary, it is perfectly fine to go back and edit the `PLAN.md` file. The key is that the plan always reflects the current state of the project.

# Frontend Development Guidelines (gemini.md)

This document outlines the coding standards, conventions, and best practices for frontend development in this project. Adhering to these guidelines ensures our codebase is readable, consistent, and maintainable.

## Table of Contents
1.  [General](#general)
2.  [HTML](#html)
3.  [CSS](#css)
4.  [JavaScript](#javascript)
5.  [API Communication](#api-communication)

---

## General

### 1. File and Folder Structure

All frontend assets and source files should be organized according to the following structure:

```
project-root/
├── index.html
├── assets/
│   ├── images/
│   │   └── example.png
│   └── fonts/
├── css-styles/
│   └── main.css
└── js-tools/
    └── app.js
```

-   **`index.html`**: The main HTML entry point resides in the root.
-   **`assets/`**: Contains all static assets like images, fonts, and icons.
-   **`css-styles/`**: Contains all custom CSS files.
-   **`js-tools/`**: Contains all JavaScript files.

### 2. Performance Optimization

-   **Image Optimization**: All images must be optimized for the web. Use appropriate formats (e.g., WebP, AVIF) and compress images to reduce file size without significant quality loss.
-   **Code Minification**: Before deployment, all HTML, CSS, and JavaScript files must be minified to reduce their file size and improve load times.

### 3. Recommended Tooling

To enforce code style and catch errors early, we recommend the following tools:

-   **Code Formatting**: [Prettier](https://prettier.io/) for automatically formatting HTML, CSS, and JavaScript.
-   **JavaScript Linting**: [ESLint](https://eslint.org/) configured with the `eslint-config-google` preset to follow the Google JavaScript Style Guide.
-   **CSS Linting**: [Stylelint](https://stylelint.io/) to enforce consistency and avoid errors in our stylesheets.

---

## HTML

### 1. Indentation and Formatting

-   Readability is the top priority. Use default indentation (typically 2 or 4 spaces) for nested elements to ensure the code is easy to scan and understand.

### 2. Naming Conventions

-   Class and ID names should be derived directly from the content or purpose of the element.
-   Use lowercase letters and separate words with hyphens (`-`).

**Example:**
-   A section about the company's services: `<div class="about-services">...</div>`
-   A paragraph with the text "Watch MLS and Liga Mx kick off Leagues Cup today": `<p class="watch-leagues">...</div>`

### 3. Comments

-   **Clarity and Conciseness**: Write clear and brief comments that explain the *why*, not the *what*.
-   **Avoid Over-Commenting**: Do not comment on every line. Focus on logic that isn't self-explanatory.
-   **No Sensitive Information**: Never include credentials, API keys, or other sensitive data in HTML comments.

### 4. Accessibility (A11y)

-   Use ARIA (Accessible Rich Internet Applications) roles where necessary to enhance accessibility for screen readers and other assistive technologies.

**Example:**
```html
<nav role="navigation">
  ...
</nav>
```

---

## CSS

### 1. Methodology: Tailwind First

-   Always prioritize using [Tailwind CSS](https://tailwindcss.com/) for styling and layout.
-   Build for **mobile-first responsiveness**. Start with mobile styles and use Tailwind's responsive prefixes (e.g., `sm:`, `md:`, `lg:`) to add styles for larger screens.
-   Only write custom CSS in the `css-styles/` directory for styles that cannot be achieved with Tailwind utility classes (e.g., complex animations).

### 2. Custom CSS Selectors

-   **Order**: Custom CSS rules should be ordered to match the visual layout of the page (e.g., `.header`, `.navigation`, `.main-content`, `.footer`).
-   **Naming Convention**: Class selectors must be written in lowercase with words separated by a hyphen (`-`).

    **Example:**
    ```css
    .page-header { ... }
    .contact-form-button { ... }
    ```

### 3. Units

-   **Layout and Spacing**: Use `rem` units for margins, padding, width, and height.
-   **Typography**: Use `em` units for font sizes.

---

## JavaScript

### 1. Style Guide

-   All JavaScript code must adhere to the [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html). Use ESLint to enforce these rules automatically.

### 2. Variable Declaration

-   Declare all variables with `const` by default.
-   Only use `let` if the variable's value needs to be reassigned later. Avoid using `var`.

### 3. Comments

-   **Simple Functions**: A single, concise one-liner explaining the function's purpose is sufficient.
-   **Complex Functions**: If a function involves multiple steps or complex logic, provide a summary followed by numbered steps explaining the overall process.

### 4. Semicolons

-   Always use semicolons at the end of statements.

### 5. Modules

-   Use ES6 modules (`import`/`export`) for organizing and sharing code between files.

---

## API Communication

All network requests must handle the three core states of an API call to ensure a good user experience and aid in debugging.

### 1. Loading State

-   **Action**: While data is being fetched from the API, a clear visual indicator, such as a loading bar or spinner, must be displayed to the user.
-   **Purpose**: This provides feedback that the application is working and prevents the user from thinking the page is frozen.

### 2. Success State

-   **Action**: Upon a successful API response, the fetched data should be rendered to the user. For debugging purposes, the success status and/or data should be logged to the console.
-   **Purpose**: Confirms that the data was fetched correctly and allows developers to inspect the response.

    **Example:**
    ```javascript
    fetch('api/data')
      .then(response => response.json())
      .then(data => {
        console.log('Success:', data); // For debugging
        // Render data to the UI
      });
    ```

### 3. Error State

-   **Action**: If an API request fails or returns an error, the error message must be logged to the console. A user-friendly error message should be displayed in the UI.
-   **Purpose**: Crucial for debugging. Logging the raw error helps developers pinpoint the issue, while a friendly message informs the user without causing confusion.

    **Example:**
    ```javascript
    fetch('api/data').catch(error => {
      console.error('API Error:', error); // For debugging
      // Display a user-friendly message, e.g., "Could not load data."
    });
    ```