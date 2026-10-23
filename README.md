# 💌 Interactive Greeting Card

<p align="center">
  <strong>A beautiful, responsive greeting card experience built with HTML5 and CSS3.</strong>
  <br />
  Explore CSS-powered navigation, decorative typography, smooth transitions, and responsive layouts — all without JavaScript.
</p>

<p align="center">
  <a href="https://regalson001.github.io/interactive-greeting-card/">
    <img src="https://img.shields.io/badge/🌐_Live_Demo-View_Project-2ea44f?style=for-the-badge" alt="View Live Demo" />
  </a>
  <img src="https://img.shields.io/badge/HTML5-Structure-e34f26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-Styling-1572b6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
</p>

---

## 🌐 Live Demo

**Experience the project in your browser:**

👉 [View the Interactive Greeting Card](https://regalson001.github.io/interactive-greeting-card/)

## 🖼️ Preview

![Interactive Greeting Card Preview](preview.png)

> **Preview image:** Add a screenshot named `preview.png` to the root of your repository. If your screenshot has a different filename or is stored in another directory, update the image path accordingly.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [How It Works](#-how-it-works)
- [Responsive Design](#-responsive-design)
- [Accessibility and Best Practices](#-accessibility-and-best-practices)
- [Learning Objectives](#-learning-objectives)
- [Project Limitations](#-project-limitations)
- [Future Improvements](#-future-improvements)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

## 🎯 Overview

The **Interactive Greeting Card** is a front-end web development project designed to demonstrate how a simple web page can become an engaging, interactive experience through thoughtful HTML structure and modern CSS techniques.

The project presents greeting card content in a clean, visually appealing layout. It explores CSS fragment-based navigation, pseudo-classes, pseudo-elements, transitions, and Flexbox to create an interface that is responsive, maintainable, and easy to explore.

Built entirely with HTML5 and CSS3, the project provides practical experience in creating interactive web components without relying on JavaScript or external frameworks.

### Project Goals

- Build a structured interface using semantic HTML5.
- Create a visually appealing greeting card with CSS3.
- Explore CSS `:target` for fragment-based navigation.
- Use pseudo-classes to style link interaction states.
- Apply pseudo-elements for decorative visual effects.
- Develop responsive layouts using Flexbox and media queries.
- Practise accessibility, maintainability, and clean code organization.

## ✨ Features

- **CSS-Powered Navigation:** Uses the `:target` pseudo-class to navigate between card sections through URL fragments.
- **Decorative Typography:** Uses `::before` and `::after` pseudo-elements to add visual details to headings and other elements.
- **Interactive Link Styling:** Provides visual feedback with `:hover`, `:active`, `:focus-visible`, and `:visited`.
- **Responsive Layout:** Uses flexible CSS layouts to support desktop, tablet, and mobile viewports.
- **Smooth Transitions:** Adds subtle transitions to supported visual properties.
- **Modern Visual Design:** Combines typography, spacing, colors, and decorative details to create a polished appearance.
- **Semantic HTML5:** Organizes content using meaningful structural elements.
- **JavaScript-Free Implementation:** Demonstrates the CSS-based interactions implemented in the project without requiring JavaScript.
- **Lightweight Setup:** Runs directly in a modern web browser without installing dependencies.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Structures the greeting card content and navigation. |
| CSS3 | Controls visual styling, layout, and transitions. |
| CSS Flexbox | Aligns and positions interface elements. |
| CSS Pseudo-Classes | Styles interaction states and target-based sections. |
| CSS Pseudo-Elements | Creates decorative content and visual accents. |
| CSS Media Queries | Adjusts layouts for different viewport sizes. |
| Git and GitHub | Supports version control and project hosting. |
| GitHub Pages | Hosts the live project demo. |

## 📂 Project Structure

```text
interactive-greeting-card/
│
├── index.html      # Main HTML structure and card content
├── styles.css      # Styling, layout, and CSS interactions
├── preview.png     # README preview screenshot
└── README.md       # Project documentation
```

The `preview.png` file is used for documentation. If you choose not to include a screenshot, remove the preview image reference from this README.

## 🚀 Getting Started

Run the project locally in a few simple steps.

### Prerequisites

You need:

- A modern web browser.
- A code editor, such as Visual Studio Code, for modifying the source files.
- Git, if you want to clone the repository.

No JavaScript runtime, package manager, or build tool is required.

### 1. Clone the Repository

```bash
git clone https://github.com/Regalson001/interactive-greeting-card.git
```

### 2. Navigate to the Project Directory

```bash
cd interactive-greeting-card
```

### 3. Open the Project

Open `index.html` directly in your browser.

Alternatively, open the project folder in Visual Studio Code and use the Live Server extension for a convenient development preview.

### 4. Explore and Customize

Edit `index.html` to change greeting messages, headings, and card sections.

Edit `styles.css` to customize colors, typography, spacing, layout, transitions, and responsive behavior.

Save your changes and refresh the browser to see the updated design.

## 💡 How It Works

### 1. HTML5 Structure

Semantic HTML elements organize the greeting card content and make the document easier to understand and maintain.

Typical elements include:

- `<header>` for introductory content.
- `<nav>` for navigation links.
- `<main>` for the primary page content.
- `<section>` for individual greeting cards.
- Heading elements for a logical content hierarchy.

Use each element according to its semantic purpose.

### 2. CSS `:target` Navigation

The `:target` pseudo-class selects an element whose ID matches the fragment identifier in the current URL.

For example:

```html
<nav aria-label="Greeting navigation">
  <a href="#birthday">Birthday</a>
  <a href="#thank-you">Thank You</a>
</nav>

<section id="birthday">
  <h2>Happy Birthday!</h2>
  <p>Wishing you a wonderful celebration.</p>
</section>

<section id="thank-you">
  <h2>Thank You!</h2>
  <p>Your kindness means so much.</p>
</section>
```

CSS can use these fragment links to display the selected section:

```css
section {
  display: none;
}

section:target {
  display: block;
}
```

This is an illustrative example. A complete implementation should also account for the default view when no fragment is present and ensure that the navigation and section visibility rules match the actual page structure.

### 3. CSS Pseudo-Elements

The `::before` and `::after` pseudo-elements add decorative content without requiring extra HTML elements.

```css
.card-title::before {
  content: "✦ ";
}

.card-title::after {
  content: " ✦";
}
```

These techniques can create simple visual accents around headings and other elements.

### 4. Interactive Link States

CSS pseudo-classes style links according to their interaction state.

```css
.card-link:hover {
  opacity: 0.85;
}

.card-link:focus-visible {
  outline: 3px solid currentColor;
  outline-offset: 4px;
}

.card-link:active {
  transform: scale(0.98);
}
```

These styles provide pointer feedback, keyboard focus visibility, and a subtle pressed effect.

The `:visited` pseudo-class can also be used to style previously visited links, subject to browser privacy restrictions.

### 5. Responsive Layouts

Flexbox and media queries allow the layout to adapt to available screen space.

```css
.card-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  gap: 1.5rem;
}

@media (max-width: 600px) {
  .card-container {
    flex-direction: column;
  }
}
```

This is an example of responsive styling. Adapt the selectors and breakpoint to match the actual project stylesheet.

## 📱 Responsive Design

The project is designed to provide a consistent experience across different screen sizes.

Responsive design considerations include:

- **Flexible Layouts:** Use Flexbox and relative sizing to reduce dependence on fixed dimensions.
- **Mobile-Friendly Spacing:** Adjust margins, padding, and gaps for smaller screens.
- **Readable Typography:** Maintain comfortable font sizes and line heights.
- **Flexible Card Dimensions:** Prevent content from overflowing narrow viewports.
- **Responsive Navigation:** Ensure navigation links remain visible and usable on touch devices.
- **Motion Preferences:** Respect reduced-motion preferences when transitions or animations are used.

Test the finished project on desktop, tablet, and mobile viewports to verify its behavior.

## ♿ Accessibility and Best Practices

Accessibility helps make the greeting card usable by a wider range of people.

Recommended practices include:

- Use semantic HTML elements appropriately.
- Maintain a logical heading hierarchy.
- Give navigation links descriptive labels.
- Ensure sufficient text and background contrast.
- Provide visible keyboard focus indicators.
- Keep decorative symbols from replacing meaningful text.
- Ensure that navigation works using a keyboard.
- Use responsive layouts that support browser zoom.
- Respect `prefers-reduced-motion` for non-essential animations.
- Keep HTML and CSS organized and easy to maintain.

## 🎓 Learning Objectives

This project provides practical experience with:

- Semantic HTML5 structure.
- CSS Flexbox and responsive layouts.
- Fragment-based navigation using `:target`.
- CSS pseudo-classes and pseudo-elements.
- Link interaction states.
- CSS transitions and visual feedback.
- Media queries and flexible sizing.
- Accessibility fundamentals.
- Separation of HTML structure and CSS presentation.
- GitHub project documentation and deployment.

## ⚠️ Project Limitations

This version uses HTML5 and CSS3 without JavaScript. Its interactive capabilities therefore depend on native browser behavior and the CSS rules implemented.

- Navigation through `:target` depends on matching URL fragments and element IDs.
- Greeting messages are defined in the HTML rather than generated dynamically.
- There is no built-in greeting editor or automatic personalization system.
- Custom messages and preferences are not saved by the application.
- CSS transitions provide visual effects but do not implement application logic.

These limitations are appropriate for a project focused on foundational front-end development.

## 🔮 Future Improvements

Possible enhancements include:

- **Personalized Greetings:** Add dynamic recipient names and custom messages using JavaScript.
- **Additional Card Themes:** Create designs for birthdays, anniversaries, celebrations, and thank-you messages.
- **Advanced Animations:** Introduce optional card-opening effects and decorative motion.
- **Theme Customization:** Add alternative color palettes and visual styles.
- **Shareable Greetings:** Support sharing specific greetings through URL parameters or fragments.
- **Improved Mobile Experience:** Refine spacing and typography for smaller screens.
- **Accessibility Testing:** Evaluate keyboard navigation, contrast, and screen-reader usability.
- **Deployment Improvements:** Keep the GitHub Pages demo updated whenever the project changes.

These are potential enhancements rather than claims about existing functionality.

## 🤝 Contributing

Feedback and improvements are welcome.

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-improvement
   ```

3. Make your changes and test the project.
4. Commit your changes:

   ```bash
   git commit -m "Improve greeting card design"
   ```

5. Push your branch:

   ```bash
   git push origin feature/your-improvement
   ```

6. Open a pull request describing your improvements.

Please keep contributions focused, accessible, and consistent with the project's goals.

## 📄 License

No license has been specified for this project yet.

If you intend to distribute the project as open-source software, choose an appropriate license and add a `LICENSE` file to the repository. Until a license is added, do not assume that the source code is available for unrestricted reuse or redistribution.

## 👨‍💻 Author

**Stephen Oyugi**

- GitHub Profile: [@Regalson001](https://github.com/Regalson001)
- Project Repository: [Interactive Greeting Card](https://github.com/Regalson001/interactive-greeting-card)
- Live Demo: [View the Greeting Card](https://regalson001.github.io/interactive-greeting-card/)

---

<p align="center">
  Designed with HTML5 and CSS3.
</p>

<p align="center">
  <strong>Simple code. Thoughtful design. Meaningful greetings.</strong>
</p>
