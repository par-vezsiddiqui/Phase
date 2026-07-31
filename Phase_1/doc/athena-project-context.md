# Athena Project HTML Structure Review

## 1. Project Overview
This project is a small multi-page student portal website built as a set of static HTML pages. Its main purpose is to present student-related information such as profile details, courses, grades, feedback, and contact information in a simple, navigable structure. The project relies heavily on standard HTML page organization using elements such as `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<form>`, `<table>`, and `<footer>`. The overall structure is straightforward and consistent across all pages.

## 2. File and Page Summary

### index.html
- Purpose: Home page for the student portal.
- Main HTML elements: `<header>`, `<nav>`, `<ul>`, `<li>`, `<a>`, `<main>`, `<section>`, `<p>`, `<footer>`.
- Page structure: A simple landing page with a top navigation bar, a welcome section, and a footer.

### profile.html
- Purpose: Displays student profile information.
- Main HTML elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<img>`, `<p>`, `<ul>`, `<ol>`, `<li>`, `<footer>`.
- Page structure: Organized into several content sections for personal information, details, and hobbies/goals.

### courses.html
- Purpose: Shows a list of current courses.
- Main HTML elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<h3>`, `<p>`, `<a>`, `<footer>`.
- Page structure: Content is grouped into distinct course cards using `<article>` blocks.

### grades.html
- Purpose: Presents semester grades in a tabular layout.
- Main HTML elements: `<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<tr>`, `<th>`, `<td>`, `<header>`, `<nav>`, `<main>`, `<footer>`.
- Page structure: A single main content area containing a structured grade table.

### feedback.html
- Purpose: Provides a feedback submission form.
- Main HTML elements: `<form>`, `<label>`, `<input>`, `<select>`, `<option>`, `<textarea>`, `<button>`, `<header>`, `<nav>`, `<main>`, `<footer>`.
- Page structure: A single form-centered page with input controls grouped within a form container.

### contact.html
- Purpose: Displays contact details for the student portal support team.
- Main HTML elements: `<header>`, `<nav>`, `<main>`, `<section>`, `<address>`, `<p>`, `<a>`, `<footer>`.
- Page structure: A contact information page with a short introductory section and address/contact details.

## 3. Page Structure and Navigation
The project uses a consistent page pattern on every file: a top `<header>` with a page title and a shared `<nav>` menu, a `<main>` content area, and a `<footer>`. All pages are linked together through a navigation list that connects the home page, profile page, courses page, feedback page, grades page, and contact page.

### Navigation Structure
Each page includes a navigation block with links to:
- index.html
- profile.html
- courses.html
- feedback.html
- grades.html
- contact.html

This creates a simple cross-linked website where the user can move between all major sections from any page.

## 4. HTML Elements and Structure

### 1. `<header>`
- Used in: All pages, at the top of the document.
- Why appropriate: It is the natural container for the page title and navigation.
- Meaning and accessibility: It identifies introductory content for the page and helps users quickly understand the page context.
- Best practice: Each page uses a single clear `<h1>` inside the header, which is good structural organization.

### 2. `<nav>`
- Used in: All pages within the shared top menu.
- Why appropriate: It clearly groups the site navigation links.
- Meaning and accessibility: It communicates that the links are part of the main site navigation.
- Best practice: The navigation is placed consistently in each page header, improving predictability.

### 3. `<main>`
- Used in: All pages as the primary content container.
- Why appropriate: It marks the main body of content for each page.
- Meaning and accessibility: It helps distinguish the primary content from repeated header/footer content.
- Best practice: Each page has only one main content area, which keeps the structure clean.

### 4. `<section>`
- Used in: index.html, profile.html, and contact.html.
- Why appropriate: It groups related content into meaningful content blocks.
- Meaning and accessibility: It gives logical organization to content sections such as the welcome message, profile topics, and contact details.
- Best practice: Section headings such as `<h2>` are used inside them, which improves clarity.

### 5. `<article>`
- Used in: courses.html for each course entry.
- Why appropriate: Each course item is a self-contained content unit.
- Meaning and accessibility: It represents standalone content that could be reused or presented independently.
- Best practice: Each `<article>` contains its own heading and descriptive paragraph, making the structure readable.

### 6. `<form>`
- Used in: feedback.html.
- Why appropriate: It is the correct container for a set of form controls meant to collect user input.
- Meaning and accessibility: It clearly groups related inputs and supports a structured input submission process.
- Best practice: The form uses labels associated with inputs and a submit button, which is a strong HTML practice.

### 7. `<input>`
- Used in: feedback.html for the full name, email, and checkbox controls.
- Why appropriate: It provides different input types for collecting user information.
- Meaning and accessibility: The `type` attribute conveys the kind of data expected.
- Best practice: `id` and `name` attributes are used, and labels are paired with input elements.

### 8. `<select>` and `<option>`
- Used in: feedback.html for the rating field.
- Why appropriate: They are appropriate for choosing from a predefined list of options.
- Meaning and accessibility: They give users a compact, structured way to pick a value.
- Best practice: The field is clearly labeled and uses standard option values.

### 9. `<textarea>`
- Used in: feedback.html for comments.
- Why appropriate: It supports multiline text entry.
- Meaning and accessibility: It is semantically suited for longer written feedback.
- Best practice: The textarea is labeled and sized using attributes such as `rows` and `cols`.

### 10. `<table>`
- Used in: grades.html.
- Why appropriate: It is the correct structure for presenting tabular data such as course names, grades, and credits.
- Meaning and accessibility: It explicitly represents relationships between rows and columns.
- Best practice: The table includes `<caption>`, `<thead>`, `<tbody>`, and `<tfoot>`, which improve structure and readability.

## 5. Page Structure and Navigation

### Pages and Structure
- index.html: Home page with a welcome section and links to other pages.
- profile.html: Profile page with an image, descriptive paragraph, and lists of personal details and hobbies.
- courses.html: Course page with three course article blocks.
- grades.html: Grade page with a table of academic results.
- feedback.html: Feedback page with a form for collecting input.
- contact.html: Contact page with address and contact links.

### Navigation Links Between Pages
The navigation block in each page links to the following pages:
- Home -> index.html
- Profile -> profile.html
- Courses -> courses.html
- Feedback -> feedback.html
- Grades -> grades.html
- Contact Us -> contact.html

### Form Elements and Types
The form in feedback.html contains:
- `<input type="text">` for the full name
- `<input type="email">` for the email address
- `<select>` with `<option>` elements for rating selection
- `<textarea>` for comments
- `<input type="checkbox">` for a follow-up request
- `<button type="submit">` for submission

### Table Structure and Data Organization
The table in grades.html uses:
- `<caption>` for the table title
- `<thead>` for the header row
- `<tbody>` for the main rows of data
- `<tfoot>` for the summary row
- `<th>` for column headers
- `<td>` for cell values

### List Usage
- `<ul>` is used in the shared navigation menu and in profile.html for personal details.
- `<ol>` is used in profile.html for ordered goals/hobbies.
- `<li>` is used to define each list item in both unordered and ordered lists.

## 6. References
Students should focus on the following files to understand the project well:
- [index.html](../index.html) — shows the shared homepage layout and navigation pattern.
- [profile.html](../profile.html) — demonstrates the use of images, sections, and lists.
- [courses.html](../courses.html) — shows how article blocks can be used to organize content.
- [grades.html](../grades.html) — is the clearest example of a structured HTML table.
- [feedback.html](../feedback.html) — is the best example of form markup and input controls.
- [contact.html](../contact.html) — shows contact content organized with address and link elements.
