# Instructor Lesson Plans: 12-Week HTML & CSS Portfolio Course

**Audience:** Two high-school students  
**Level:** Beginner to intermediate  
**Duration:** 12 lessons, 60–90 minutes each  
**Core tools:** Browser, text/code editor, GitHub  
**Final product:** A responsive, multi-page personal portfolio published with GitHub Pages.

## Course teaching routine

Use this rhythm each week:
1. **Starter/retrieval (5–10 min):** Ask students to recall last week's key ideas.
2. **Teach and model (10–15 min):** Explain one or two concepts and demonstrate them live.
3. **Guided build (15–20 min):** Students follow a small example.
4. **Portfolio application (20–30 min):** Students apply the idea to their own site.
5. **Review and save (5–10 min):** Test in browser, fix one issue, commit/publish progress.
6. **Exit ticket:** Each student explains one thing learned and one thing to improve.

For a 60-minute lesson, shorten the independent challenge. For a 90-minute lesson, extend debugging and peer review.

---

## Week 1 — What is a website? Your first HTML page

**Learning intentions**
- Understand the roles of HTML, CSS and a web browser.
- Identify the basic structure of an HTML document.
- Create and open a first webpage.

**Success criteria**
- I can explain that HTML structures content and CSS styles it.
- I can create a valid HTML document with a title, heading and paragraph.
- I can open my page in a browser.

**Key vocabulary:** browser, website, HTML, element, tag, opening tag, closing tag, attribute.

**Lesson sequence**
1. Discuss websites students use and identify common parts: headings, paragraphs, images, links and navigation.
2. Explain: HTML = structure/content; CSS = appearance/layout; browser = displays the page.
3. Demonstrate `<!doctype html>`, `<html>`, `<head>`, `<title>` and `<body>`.
4. Students create `index.html` with a heading, short introduction and three interests.
5. Students change the browser tab title and add a second heading.
6. Pair-share: students describe how the browser knows which text is a heading.

**Teacher demonstration**
```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My First Website</title>
</head>
<body>
  <h1>Welcome to my website</h1>
  <p>I'm learning how to build websites with HTML.</p>
  <h2>My interests</h2>
  <p>I enjoy music, sport and creative projects.</p>
</body>
</html>
```

**Guided practice**
- Change the title to `My Portfolio`.
- Add an `<h2>` called `Things I Like`.
- Add a paragraph with two sentences.

**Independent challenge**
- Add a list of three interests using `<ul>` and `<li>`.
- Add a second paragraph explaining what the portfolio will showcase.

**Check for understanding**
- What is the difference between `<head>` and `<body>`?
- Which tag is the main page heading?
- What happens if a closing tag is missing?

**Homework/extension:** Sketch a paper layout for a portfolio home page with a header, introduction, projects preview and footer.

**Save point:** `week-01-first-page`.

---

## Week 2 — HTML structure and semantic elements

**Learning intentions**
- Organise content with headings, paragraphs and lists.
- Use semantic page sections.
- Build a clear About Me content outline.

**Success criteria**
- I use headings in a logical order.
- I can explain the purpose of `header`, `nav`, `main`, `section` and `footer`.
- My page content is organised into meaningful sections.

**Key vocabulary:** semantic HTML, header, navigation, main, section, footer, ordered list, unordered list.

**Lesson sequence**
1. Review Week 1: students identify the HTML document sections.
2. Introduce semantic elements and explain that they describe the purpose of content.
3. Demonstrate a page skeleton using `header`, `nav`, `main`, `section` and `footer`.
4. Students create a structured profile page.
5. Students add a short biography, interests and learning goals.
6. Peer check: can another person understand the page structure by reading the HTML?

**Worked example**
```html
<header>
  <h1>Alex's Portfolio</h1>
  <p>Student • Creator • Problem Solver</p>
</header>

<nav aria-label="Main navigation">
  <a href="index.html">Home</a>
  <a href="about.html">About</a>
</nav>

<main>
  <section>
    <h2>About Me</h2>
    <p>I enjoy learning new skills and making things.</p>
  </section>
</main>

<footer>
  <p>Portfolio project</p>
</footer>
```

**Guided practice**
- Add a section titled `My Interests`.
- Add a list of three interests.
- Add a section titled `My Goals` with two goals.

**Independent challenge**
- Create `about.html` using the starter template.
- Include a biography, interests, strengths and a learning goal.
- Use at least one `<h1>`, two `<h2>` headings, paragraphs and a list.

**Differentiation**
- Support: provide a heading outline before students write HTML.
- Extension: add an ordered list describing a process or achievement.

**Check for understanding**
- Why should a page normally have one clear main heading?
- How is `<section>` different from `<div>`?
- Why is semantic HTML helpful?

**Save point:** `week-02-semantic-html`.

---

## Week 3 — Links, images and navigation

**Learning intentions**
- Add links between pages and to external websites.
- Display images with meaningful alternative text.
- Build consistent navigation.

**Success criteria**
- All internal navigation links work.
- Images have useful `alt` text.
- Students can distinguish relative links from external URLs.

**Key vocabulary:** anchor, `href`, image, `src`, alt text, relative path, external link.

**Lesson sequence**
1. Review semantic structure.
2. Demonstrate `<a href="">` and `<img src="" alt="">`.
3. Explain relative paths such as `about.html` and `assets/photo.jpg`.
4. Students add navigation links to Home and About.
5. Add a teacher-approved image or copyright-safe image from a permitted source.
6. Test every link and image.

**Worked example**
```html
<a href="about.html">Learn more about me</a>

<img src="assets/project-one.jpg"
     alt="A small model bridge built for a design project">

<a href="https://www.example.com" target="_blank" rel="noopener">
  Visit an external website
</a>
```

**Guided practice**
- Add Home, About, Projects and Contact links to the navigation.
- Add an image with descriptive alt text.
- Add one external link to a learning resource.

**Independent challenge**
- Create a `projects.html` page with two project previews.
- Each preview should include a heading, short description and image.
- Add a link from each preview to a project detail section or approved external demonstration.

**Digital citizenship**
- Only use images students have permission to use.
- Avoid publishing identifiable personal information.
- Do not add private contact details or personal social links.

**Check for understanding**
- What does `href` do?
- Why is alt text important?
- What does a relative file path refer to?

**Save point:** `week-03-links-images`.

---

## Week 4 — Introduction to CSS

**Learning intentions**
- Explain the relationship between HTML and CSS.
- Connect an external stylesheet.
- Use selectors and declarations.

**Success criteria**
- The HTML file links to `css/style.css`.
- Students can style body text, headings and links.
- Students can identify selector, property and value.

**Key vocabulary:** stylesheet, selector, declaration, property, value, class, external CSS.

**Lesson sequence**
1. Show the same HTML page with and without CSS.
2. Explain the CSS rule pattern: selector `{ property: value; }`.
3. Demonstrate linking a stylesheet in the HTML `<head>`.
4. Students style body background, font, text colour and heading colour.
5. Introduce class selectors with `.card`.
6. Students compare designs and explain which choices improve readability.

**Worked example**
```html
<link rel="stylesheet" href="css/style.css">
```
```css
body {
  font-family: Arial, sans-serif;
  background-color: #f4f6fb;
  color: #202536;
}

h1 {
  color: #3157a4;
}

.card {
  background-color: white;
  padding: 20px;
}
```

**Guided practice**
- Change the page background.
- Set a readable font.
- Style all `h1` headings.
- Add a class named `highlight` to one paragraph and style it.

**Independent challenge**
- Create a simple visual theme with two main colours and one accent colour.
- Apply the same stylesheet to all existing pages.

**Check for understanding**
- What is the difference between a class selector and an element selector?
- Why use an external stylesheet?
- What happens if the CSS path is incorrect?

**Save point:** `week-04-first-css`.

---

## Week 5 — Colour, typography and design principles

**Learning intentions**
- Use colour and typography consistently.
- Understand contrast, spacing and visual hierarchy.
- Create a simple design system.

**Success criteria**
- Students choose a small, consistent colour palette.
- Text is readable and headings have clear hierarchy.
- Repeated elements share consistent styles.

**Key vocabulary:** typography, contrast, hierarchy, palette, font family, font size, line height.

**Lesson sequence**
1. Compare two sample pages: one cluttered, one with clear hierarchy.
2. Discuss readability, contrast, alignment and whitespace.
3. Demonstrate hex colours, font stacks, `font-size`, `font-weight` and `line-height`.
4. Students choose a theme and record colours and typography in a mini style guide.
5. Apply the theme to headings, paragraphs, links and buttons.
6. Pair review: identify one design strength and one improvement.

**Worked example**
```css
:root {
  --colour-ink: #202536;
  --colour-brand: #3157a4;
  --colour-accent: #f2a65a;
  --colour-surface: #ffffff;
  --colour-page: #f4f6fb;
}

body {
  color: var(--colour-ink);
  background: var(--colour-page);
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

h1, h2 {
  color: var(--colour-brand);
}
```

**Guided practice**
- Create three CSS variables for colours.
- Apply one font family to the whole site.
- Make headings visually distinct from body text.
- Check contrast and avoid very small text.

**Independent challenge**
- Create a mini style guide at the top of `style.css`.
- Restyle all pages so they feel like one website.
- Add a consistent button style.

**Check for understanding**
- What is visual hierarchy?
- Why is strong text contrast important?
- What is the benefit of CSS variables?

**Save point:** `week-05-design-system`.

---

## Week 6 — The CSS Box Model and spacing

**Learning intentions**
- Understand content, padding, border and margin.
- Control width and spacing.
- Use `box-sizing` to make layouts easier to manage.

**Success criteria**
- Students can explain the four parts of the box model.
- Cards have consistent padding and spacing.
- The layout does not overflow unnecessarily.

**Key vocabulary:** content, padding, border, margin, width, `box-sizing`.

**Lesson sequence**
1. Draw a box model diagram on the board.
2. Demonstrate how padding and margin change a card.
3. Introduce `box-sizing: border-box`.
4. Students build a profile card and project card.
5. Adjust width, padding, border radius and margin.
6. Inspect the page at different browser widths.

**Worked example**
```css
* {
  box-sizing: border-box;
}

.card {
  width: 100%;
  max-width: 420px;
  padding: 24px;
  margin: 16px 0;
  border: 1px solid #d9deea;
  border-radius: 14px;
  background: white;
}
```

**Guided practice**
- Add padding to a card.
- Add a border and rounded corners.
- Adjust the margin between two cards.
- Use `max-width` to stop a text section becoming too wide.

**Independent challenge**
- Create a reusable `.card` style.
- Use it for at least two sections.
- Make the main content centred with a maximum width.

**Check for understanding**
- How is margin different from padding?
- What does `border-box` change?
- Why might `max-width` be useful?

**Save point:** `week-06-box-model`.

---

## Week 7 — Flexbox and CSS Grid

**Learning intentions**
- Arrange content using Flexbox.
- Build a project gallery using CSS Grid.
- Choose a layout tool suited to the task.

**Success criteria**
- Navigation items are aligned using Flexbox.
- Project cards display in a grid.
- The layout adapts when the browser width changes.

**Key vocabulary:** flex container, flex item, justify-content, align-items, grid, columns, gap.

**Lesson sequence**
1. Demonstrate a row of items using `display: flex`.
2. Introduce `justify-content`, `align-items`, `gap` and `flex-wrap`.
3. Demonstrate a two/three-column project grid with CSS Grid.
4. Students build a project gallery with three cards.
5. Adjust the number of columns for narrower screens.
6. Test and compare Flexbox and Grid.

**Worked example**
```css
.navigation {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 16px;
  flex-wrap: wrap;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}
```

**Guided practice**
- Use Flexbox to align navigation links.
- Use Grid to create three project columns.
- Add a gap between cards.

**Independent challenge**
- Create a gallery of at least three projects.
- Make cards align neatly even if descriptions have different lengths.
- Add a media query that changes the grid to one column on small screens.

**Differentiation**
- Support: use `repeat(2, 1fr)` and then change it to one column.
- Extension: use `minmax()` and `auto-fit` to create a flexible grid.

**Check for understanding**
- When might Flexbox be a good choice?
- When might Grid be a better choice?
- What does `gap` do?

**Save point:** `week-07-flexbox-grid`.

---

## Week 8 — Multiple pages and reusable components

**Learning intentions**
- Plan a consistent multi-page website.
- Reuse navigation, header and footer patterns.
- Connect all portfolio pages.

**Success criteria**
- Home, About, Projects and Contact pages exist.
- Navigation is consistent on every page.
- No internal links are broken.

**Key vocabulary:** multi-page site, reusable pattern, relative path, information architecture.

**Lesson sequence**
1. Map the four pages and decide what content belongs on each.
2. Demonstrate copying a shared header/navigation/footer structure.
3. Students create or complete all four HTML files.
4. Apply the same CSS file to every page.
5. Add a clear page heading and meaningful content to each page.
6. Test every navigation link from every page.

**Page content checklist**
- Home: introduction, short tagline, featured projects.
- About: biography, interests, learning goals.
- Projects: at least three project cards.
- Contact: safe, teacher-approved contact option or a non-functional demonstration contact layout.

**Guided practice**
- Copy the navigation into each page.
- Update the active page link or add a simple active-page class.
- Add a footer to each page.

**Independent challenge**
- Add a `project-one.html` detail page or a detailed project section.
- Include the problem, process, tools and outcome.
- Ensure a visitor can return to the Projects page.

**Check for understanding**
- Why should navigation stay consistent?
- What is a relative path?
- How can you test a multi-page site?

**Save point:** `week-08-multi-page`.

---

## Week 9 — Advanced CSS: hover states, transitions and polish

**Learning intentions**
- Use pseudo-classes such as `:hover` and `:focus`.
- Add transitions and subtle visual feedback.
- Improve usability without distracting effects.

**Success criteria**
- Links and buttons have visible hover and keyboard-focus states.
- Transitions are subtle and purposeful.
- Interactive elements remain readable and usable.

**Key vocabulary:** pseudo-class, hover, focus, transition, transform, state.

**Lesson sequence**
1. Demonstrate hover and focus states.
2. Explain that keyboard users also need visible focus.
3. Add transitions to buttons and project cards.
4. Students style navigation and project cards.
5. Test by using mouse and keyboard.
6. Review whether effects help or distract.

**Worked example**
```css
.button {
  display: inline-block;
  padding: 10px 16px;
  color: white;
  background: #3157a4;
  border-radius: 8px;
  text-decoration: none;
  transition: background-color 180ms ease, transform 180ms ease;
}

.button:hover {
  background: #223f7d;
  transform: translateY(-2px);
}

.button:focus-visible {
  outline: 3px solid #f2a65a;
  outline-offset: 3px;
}
```

**Guided practice**
- Add a hover colour to navigation links.
- Add a subtle hover effect to project cards.
- Add a focus-visible outline to links and buttons.

**Independent challenge**
- Create a consistent button style for all pages.
- Add a small transition to cards.
- Check that all effects still work without a mouse.

**Check for understanding**
- What is a pseudo-class?
- Why should keyboard focus be visible?
- Why should transitions be subtle?

**Save point:** `week-09-interactions`.

---

## Week 10 — Responsive web design

**Learning intentions**
- Understand why websites need to work on different screen sizes.
- Use flexible widths and media queries.
- Test a site at mobile, tablet and desktop widths.

**Success criteria**
- No horizontal scrolling at common mobile widths.
- Navigation and project cards fit small screens.
- Images scale within their containers.

**Key vocabulary:** responsive design, viewport, media query, breakpoint, fluid width.

**Lesson sequence**
1. Show a desktop layout on a narrow screen and identify problems.
2. Demonstrate `max-width: 100%`, flexible containers and media queries.
3. Add a mobile breakpoint.
4. Students test using browser developer tools.
5. Fix overflowing content and cramped navigation.
6. Peer test on at least two viewport sizes.

**Worked example**
```css
img {
  max-width: 100%;
  height: auto;
}

.container {
  width: min(100% - 32px, 1000px);
  margin-inline: auto;
}

@media (max-width: 700px) {
  .project-grid {
    grid-template-columns: 1fr;
  }

  .navigation {
    justify-content: center;
  }
}
```

**Guided practice**
- Make images responsive.
- Change project grid to one column below 700px.
- Reduce large heading sizes on small screens if needed.

**Independent challenge**
- Test the full website at approximately 375px, 768px and 1280px wide.
- Fix at least three responsive issues.
- Record what changed and why.

**Check for understanding**
- What is a media query?
- Why use flexible widths?
- What causes horizontal scrolling?

**Save point:** `week-10-responsive`.

---

## Week 11 — Final portfolio build and debugging

**Learning intentions**
- Combine HTML and CSS skills in a complete project.
- Debug common problems systematically.
- Use feedback to improve a website.

**Success criteria**
- All required pages and sections are complete.
- Links and images work.
- The website is responsive and visually consistent.
- Students can explain important parts of their code.

**Lesson sequence**
1. Review the final project checklist and rubric.
2. Students complete missing content and project descriptions.
3. Teacher demonstrates a debugging routine: inspect file names/paths, check tags, inspect CSS selectors, use browser developer tools.
4. Students test every page and fix issues.
5. Partner review using the rubric.
6. Students make at least two improvements based on feedback.

**Final project checklist**
- [ ] Home page with introduction
- [ ] About page with biography/interests
- [ ] Projects page with at least three projects
- [ ] Contact page with safe contact approach
- [ ] Shared navigation and footer
- [ ] External stylesheet linked on all pages
- [ ] Consistent colours and typography
- [ ] Responsive layout
- [ ] Images have alt text
- [ ] Links and file paths tested
- [ ] No private personal information published

**Independent challenge**
- Add one original feature such as a timeline, featured project, skills display or custom illustration.
- Explain how the feature is built using HTML and CSS.

**Check for understanding**
- What was the most difficult bug you fixed?
- How did you test the site?
- What improvement made the biggest difference?

**Save point:** `week-11-final-draft`.

---

## Week 12 — GitHub Pages, presentation and reflection

**Learning intentions**
- Publish a static website with GitHub Pages.
- Present design decisions and explain code.
- Reflect on progress and next steps.

**Success criteria**
- The portfolio is accessible through its published GitHub Pages URL.
- Students can explain their page structure and CSS choices.
- Students can identify a future improvement.

**Lesson sequence**
1. Explain repositories, commits and publishing in simple terms.
2. Check that `index.html` is in the repository root.
3. Demonstrate repository Settings → Pages and select the publishing source/branch according to the current GitHub interface.
4. Students enable GitHub Pages and wait for deployment.
5. Test the live website on a second device or browser.
6. Each student gives a 3–5 minute presentation.

**Presentation prompts**
- What is the purpose of your portfolio?
- Which page are you most proud of?
- Show one HTML feature and one CSS feature you built.
- What was one problem you solved?
- What would you add with another two weeks?

**Final submission**
- GitHub repository link
- Published website link
- Short reflection (150–250 words)
- Final project rubric

**Teacher note:** GitHub's interface may change. Use GitHub's current Pages documentation if menu labels differ. A static HTML/CSS portfolio does not require a backend or server-side code.

**Save point:** `week-12-published`.
