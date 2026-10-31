## Assignment 7.5 — Flexbox Mini-Project

### 1. `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Landing Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav class="navbar">
        <h2>WebTech</h2>
        <div class="links">
            <a href="#">Home</a>
            <a href="#features">Features</a>
            <a href="#contact">Contact</a>
        </div>
        <a class="button" href="#contact">Get Started</a>
    </nav>

    <section class="hero">
        <div>
            <h1>Build Your Future Online</h1>
            <p>Learn skills and create amazing websites with us.</p>
            <a class="button" href="#features">Explore More</a>
        </div>
        <img src="https://placehold.co/400x250?text=Web+Development"
             alt="Web development illustration">
    </section>

    <section id="features">
        <h2>Our Features</h2>
        <div class="features">
            <div class="card">
                <h3>Easy Learning</h3>
                <p>Learn web development step by step.</p>
            </div>
            <div class="card">
                <h3>Practical Projects</h3>
                <p>Build real projects to improve your skills.</p>
            </div>
            <div class="card">
                <h3>Responsive Design</h3>
                <p>Create websites for mobile and desktop.</p>
            </div>
        </div>
    </section>

    <section class="cta" id="contact">
        <h2>Start Learning Today!</h2>
        <p>Take the first step toward your web development journey.</p>
        <a class="button" href="mailto:hello@example.com">Contact Us</a>
    </section>

    <footer>
        <p>© 2026 WebTech. All rights reserved.</p>
    </footer>
</body>
</html>
```

### 2. `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f4f7fb;
    color: #333;
    line-height: 1.6;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
    padding: 15px 6%;
    background: #123c69;
    color: white;
}

.links {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

.links a {
    color: white;
    text-decoration: none;
}

.button {
    display: inline-block;
    background: #ff9800;
    color: white;
    padding: 10px 18px;
    border-radius: 6px;
    text-decoration: none;
}

.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 30px;
    padding: 60px 8%;
}

.hero div,
.hero img {
    flex: 1 1 280px;
    min-width: 0;
}

.hero img {
    max-width: 100%;
    border-radius: 10px;
}

#features {
    padding: 30px 8%;
    text-align: center;
}

.features {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 20px;
}

.card {
    flex: 1 1 220px;
    min-width: 0;
    padding: 25px;
    background: white;
    border-radius: 10px;
    box-shadow: 0 3px 10px #ddd;
}

.cta {
    text-align: center;
    background: #dce8f5;
    padding: 40px 20px;
}

footer {
    text-align: center;
    background: #123c69;
    color: white;
    padding: 15px;
}

@media (max-width: 600px) {
    .navbar {
        flex-direction: column;
    }

    .hero {
        flex-direction: column;
        text-align: center;
        padding: 35px 20px;
    }
}
```

### 3. GitHub Repository

1. Create a public repository named `flexbox-landing-page` on [GitHub](https://github.com/).
2. Upload `index.html` and `style.css`.
3. Copy your repository URL for submission.

**Design explanation:** Flexbox aligns the navbar, hero, and feature cards. Consistent colors and spacing create a clean design. `flex-wrap` makes cards responsive, while the media query improves the mobile layout.