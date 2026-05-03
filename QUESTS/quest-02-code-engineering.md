# Quest 2 — Code & Engineering

**Sphere:** T | **Time:** 2-4 hours | **Difficulty:** Beginner-friendly

---

## Scenario

You're the newest developer at a small agency. Your first assignment: build a personal portfolio page from scratch — HTML, CSS, and a tiny bit of JavaScript. No frameworks. No templates. Just you and the code.

---

## Theory Bite

Software engineering is **problem-solving with code**. The daily reality:

1. **Understand** the requirement (what should this do?)
2. **Plan** the structure (how will it work?)
3. **Write** code (translate the plan into instructions)
4. **Debug** (fix what doesn't work — this is most of the job)
5. **Iterate** (improve, refactor, extend)

Key truth: **you will spend more time reading and debugging code than writing it.** If you enjoy the puzzle of "why doesn't this work?", this might be your path.

Core tools: text editor/IDE, Git, browser dev tools, terminal

---

## Hands-On Task

### Part 1: Build the Structure (30 min)

Create an `index.html` file with:
- A header with your name
- An "About Me" section
- A "Projects" section with 3 placeholder project cards
- A "Contact" section with a simple form (name, email, message)

No styling yet — just raw HTML. Open it in a browser. It'll look ugly. That's fine.

### Part 2: Add Style (45 min)

Create a `style.css` file and link it. Make the page:
- Centered layout (max-width: 800px)
- A color scheme you choose (pick 2-3 colors)
- Project cards in a grid or flexbox layout
- Hover effects on the project cards
- A responsive design that works on mobile

### Part 3: Add Interactivity (30 min)

Add a `script.js` file:
- When the form is submitted, show an alert saying "Message sent!" (prevent default)
- Add a "dark mode" toggle button
- Add a smooth scroll when clicking navigation links

### Part 4: Deploy It (30 min)

Push your code to a GitHub repository and enable GitHub Pages. Your site should be live at `https://yourusername.github.io/your-repo-name/`.

<details>
<summary>Stuck? Click here for HTML starter</summary>

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <header>
    <h1>Your Name</h1>
    <p>Aspiring Developer</p>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p>Write something about yourself here.</p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="project-grid">
      <div class="card">
        <h3>Project 1</h3>
        <p>Description of project 1</p>
      </div>
      <div class="card">
        <h3>Project 2</h3>
        <p>Description of project 2</p>
      </div>
      <div class="card">
        <h3>Project 3</h3>
        <p>Description of project 3</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your name" required>
      <input type="email" placeholder="Your email" required>
      <textarea placeholder="Your message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <script src="script.js"></script>
</body>
</html>
```

</details>

---

## Reflection Questions

- Did you enjoy the process of building something from nothing?
- How did you feel when something didn't work and you had to debug it — frustrated or challenged?
- Did you care more about how it looks (design) or how it works (engineering)?
- Could you see yourself doing this 8 hours a day?

---

## Verdict

| If this describes you | Flag |
|-----------------------|------|
| You kept adding features beyond the task | Green |
| Debugging felt like a puzzle, not a chore | Green |
| You cared about the visual result more than the code | Yellow (maybe Design & UX instead) |
| You hated debugging and wanted it to "just work" | Red |
| The blank page was exciting, not scary | Green |
