# Project Plan: WebCraft Plaza Website

**Goal:** To build a single-page marketing website for the company "WebCraft Plaza" to showcase their services, display their work, and attract potential clients.

---

## Phase 1: Project Setup & Tooling

- [ ] Create project folder structure:
  - [ ] `assets/images/`
  - [ ] `css-styles/`
  - [ ] `js-tools/`
- [ ] Create initial files:
  - [ ] `index.html`
  - [ ] `css-styles/main.css`
  - [ ] `js-tools/app.js`
- [ ] Add Tailwind CSS via CDN to `index.html`.
- [ ] Add placeholder images to `assets/images/` for the hero, services, featured work, and about sections.

---

## Phase 2: HTML Scaffolding (Structure First)

*Goal: Build the semantic HTML structure for the single page based on the provided image. No styling will be added in this phase.*

- [ ] **Header:**
    - [ ] Create `<header>` with a logo and a `<nav>` element.
    - [ ] Add navigation links: "Services", "Our Work", "About", "Testimonials", "Contact".
    - [ ] Add a "Let's Talk" call-to-action button.
- [ ] **Hero Section:**
    - [ ] Create a `<section>` for the hero.
    - [ ] Add the main heading: "Custom Software Tailored for Your UNIQUE Needs".
    - [ ] Add the list of services mentioned in the hero.
- [ ] **Services Section ("What We Help With"):**
    - [ ] Create a `<section>` for services.
    - [ ] Add a heading and a descriptive paragraph.
    - [ ] Create a grid layout for the six service cards (Graphic Design, Web Design, etc.).
    - [ ] Add content (title, description) to each service card.
- [ ] **Featured Work Section:**
    - [ ] Create a `<section>` for featured work.
    - [ ] Add a heading.
    - [ ] Create a grid to display project images.
- [ ] **Testimonials Section:**
    - [ ] Create a `<section>` for testimonials.
    - [ ] Add a heading.
    - [ ] Create containers for at least two testimonials, each with placeholder text and author.
- [ ] **About Section:**
    - [ ] Create a `<section>` for the "About WebCraft Plaza" content.
    - [ ] Add a heading and the descriptive text.
    - [ ] Add a placeholder for the team image.
- [ ] **Contact Section:**
    - [ ] Create a `<section>` for the contact form.
    - [ ] Add a heading "Get in Touch".
    - [ ] Build the HTML for the contact form (`<form>`, `<label>`, `<input>`, `<textarea>`, `<button>`).
- [ ] **Footer:**
    - [ ] Create `<footer>`.
    - [ ] Add the company logo, navigation links, and a "Let's Talk" button.

---

## Phase 3: Styling (Mobile-First with Tailwind CSS)

*Goal: Apply styles using Tailwind CSS classes to match the visual design from the `frontend.png` guide. Start with mobile views, then add responsive styles.*

- [ ] **Global Styles:**
    - [ ] Set up base font sizes, colors, and background colors in the body.
- [ ] **Components:**
    - [ ] Style the header, navigation, and "Let's Talk" buttons.
    - [ ] Style the service cards with their hover effects.
    - [ ] Style the testimonial cards.
    - [ ] Style the contact form inputs and button.
    - [ ] Style the footer.
- [ ] **Sections:**
    - [ ] Apply background colors and padding to all sections.
    - [ ] Style the typography (headings, paragraphs, lists) for each section.
    - [ ] Implement the two-column layout for the Hero and About sections.
    - [ ] Ensure all layouts are responsive and adapt to different screen sizes (`sm:`, `md:`, `lg:`).

---

## Phase 4: JavaScript & Interactivity

*Goal: Add functionality to the styled components.*

- [ ] Implement a mobile menu toggle for the navigation.
- [ ] Add smooth scrolling for internal navigation links.
- [ ] (Optional) Add simple hover effects or animations to interactive elements.
- [ ] (Optional) Add basic client-side validation for the contact form.

---

## Phase 5: Finalization & Optimization

- [ ] **Review:**
    - [ ] Proofread all content for typos.
    - [ ] Test the website on different browsers (Chrome, Firefox).
    - [ ] Test the responsive design on various screen sizes, including mobile.
- [ ] **Optimization:**
    - [ ] Ensure all images are compressed.
    - [ ] Run a Lighthouse accessibility audit and address any major issues.
- [ ] **Deployment:**
    - [ ] Prepare the final code for deployment.
