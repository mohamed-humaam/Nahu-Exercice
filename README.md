# Personal Website — 5 Pages with Separate Stylesheets

## 1) Project Structure
```
personal-site/
            ├─ index.html
            ├─ my-hobby.html
            ├─ about-me.html
            ├─ education.html
            ├─ contact.html
            └─ styles/
                    ├─ index.css
                    ├─ my-hobby.css
                    ├─ about-me.css
                    ├─ education.css
                    └─ contact.css
```

## 2) Page-to-Style Mapping
Each HTML file **must** link to its matching CSS file:
- `index.html` → `styles/index.css`
- `my-hobby.html` → `styles/my-hobby.css`
- `about-me.html` → `styles/about-me.css`
- `education.html` → `styles/education.css`
- `contact.html` → `styles/contact.css`

## 3) Content Guidelines
Add **real, personal data** for the person in each file:

- **index.html**  
  Home page — name, short tagline, 2–3 paragraph bio.

- **my-hobby.html**  
  Description of your main hobby (why you love it, how you started, photos, resources).

- **about-me.html**  
  Detailed personal intro — background, interests, values, photo (optional), fun facts.

- **education.html**  
  Schools attended, degrees, certifications, notable courses, awards, extracurriculars.

- **contact.html**  
  Email, phone (optional), social media links, and a short “open to collaboration” note.

## 4) HTML Starter Template
Use this for all pages — just change `<title>`, `<h1>`, and the stylesheet link.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Page Title</title>
  <link rel="stylesheet" href="styles/index.css" />
</head>
<body>
  <main>
    <h1>Page Heading</h1>
    <p>Replace this with your real content for this page.</p>
  </main>

  <footer>
    <small>© <span id="year"></span> Your Name</small>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
```

## 4) CSS Starter Template
Example for styles/index.css:

```css
body {
  font-family: 'Segoe UI', sans-serif;
  margin: 0;
  background: linear-gradient(135deg, #fdfbfb, #ebedee);
  color: #333;
}

main {
  max-width: 800px;
  margin: auto;
  padding: 2rem;
  text-align: center;
}

h1 {
  font-size: 2.5rem;
  color: #222;
}

footer {
  text-align: center;
  padding: 1rem;
  background: #f5f5f5;
}
```
For the other CSS files (my-hobby.css, about-me.css, education.css, contact.css), copy the above and adjust colors or layout as desired.
