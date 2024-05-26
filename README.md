# Simple Webpage

This is a simple webpage created using HTML for structure and CSS for styling. The webpage includes a header, a navigation bar, main content sections, a contact form, and a footer.

## Table of Contents

1. [Project Structure](#project-structure)
2. [Features](#features)
3. [HTML Structure](#html-structure)
4. [CSS Styling](#css-styling)
5. [How to Use](#how-to-use)

## Project Structure

The project consists of a single HTML file with internal CSS for styling.

```
simple-webpage/
├── index.html
```

## Features

- **Responsive Design**: The webpage adjusts to different screen sizes using the viewport meta tag.
- **Semantic HTML**: The use of HTML5 semantic elements for better accessibility and SEO.
- **Internal CSS**: Styles are defined within the `<style>` tag in the `<head>` section.
- **Navigation Bar**: Links to different sections of the page.
- **Contact Form**: A simple form to collect user information.

## HTML Structure

The HTML file is structured as follows:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A simple webpage using HTML and CSS">
    <title>Simple Webpage</title>
    <style>
        /* CSS goes here */
    </style>
</head>
<body>
    <header>
        <h1>Welcome</h1>
        <nav>
            <ul>
                <li class="active"><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="home">
            <h2>Home</h2>
            <p>Webpage introduction.</p>
        </section>
        <section id="about">
            <h2>About</h2>
            <article>
                <h3>About Us</h3>
                <p>Our information.</p>
            </article>
        </section>
        <section id="contact">
            <h2>Contact</h2>
            <p>Contact us using the form.</p>
            <form>
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your name" required>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required>
                <label for="message">Message:</label>
                <textarea id="message" name="message" placeholder="Enter your message" required></textarea>
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>FOOTER</p>
    </footer>
</body>
</html>
```

## CSS Styling

The CSS is defined within the `<style>` tag in the `<head>` section of the HTML file:

```css
body {
    font: 1.6em Arial, sans-serif;
    color: #0e0e0e;
    background: rgb(193, 193, 193);
    margin: 0;
    padding: 0;
}

header, footer {
    background: #4CAF50;
    color: white;
    padding: 1rem 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav li {
    display: inline;
    margin: 0 1rem;
}

nav a {
    color: rgb(226, 10, 10);
    text-decoration: none;
}

.active a {
    font-weight: bold;
    color: #ffffff;
}

main {
    padding: 2rem;
    min-height: 80vh; 
}

section {
    margin-bottom: 2rem;
}

form {
    display: flex;
    flex-direction: column;
}

form label {
    margin-bottom: 0.5rem;
}

form input, form textarea, form button {
    margin-bottom: 1rem;
    padding: 0.5rem;
    border: 1px solid #e12626;
    border-radius: 4px;
}

form input::placeholder, form textarea::placeholder {
    color: #aaa;
}

form button {
    background: #4CAF50;
    color: white;
    border: none;
    cursor: pointer;
}

form button:hover {
    background: #45a049;
}
```

## How to Use

1. Open the HTML file: Simply open `index.html` in a web browser to view the webpage.
2. Navigate: Use the navigation links to scroll to different sections of the page.
3. Submit the Form: Fill out and submit the contact form.

This project demonstrates a basic structure and styling for a simple webpage. You can expand on this foundation by adding more content, functionality, and styles as needed.
