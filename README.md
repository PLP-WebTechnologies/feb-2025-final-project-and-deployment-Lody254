<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Blog</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="hero">
      <h1>Welcome to My Blog</h1>
      <p>Sharing thoughts and ideas on technology, programming, and more!</p>
    </section>

    <section class="posts">
      <h2>Latest Posts</h2>
      <article>
        <h3>My First Post</h3>
        <p>Learn about the basics of web development in this first post...</p>
        <a href="#">Read More</a>
      </article>
      <article>
        <h3>JavaScript for Beginners</h3>
        <p>Introduction to JavaScript and how to get started...</p>
        <a href="#">Read More</a>
      </article>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 My Blog | All Rights Reserved</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>About Me | My Blog</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="about">
      <h1>About Me</h1>
      <p>Hi! I'm a passionate developer who loves coding and sharing knowledge. On this blog, I write about my learning journey and various topics in the world of web development and technology.</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 My Blog | All Rights Reserved</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>



<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Contact Me | My Blog</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="contact">
      <h1>Contact Me</h1>
      <form id="contactForm">
        <label for="name">Your Name:</label>
        <input type="text" id="name" name="name" required />

        <label for="email">Your Email:</label>
        <input type="email" id="email" name="email" required />

        <label for="message">Your Message:</label>
        <textarea id="message" name="message" rows="5" required></textarea>

        <button type="submit">Send Message</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 My Blog | All Rights Reserved</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>


body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f4f4f4;
}

header {
  background-color: #333;
  color: white;
  padding: 10px 0;
}

nav ul {
  list-style: none;
  text-align: center;
  padding: 0;
}

nav ul li {
  display: inline;
  margin: 0 20px;
}

nav ul li a {
  color: white;
  text-decoration: none;
}

.hero {
  text-align: center;
  padding: 50px 0;
}

.posts {
  padding: 20px;
}

.posts article {
  background-color: white;
  padding: 20px;
  margin: 10px 0;
}

footer {
  text-align: center;
  padding: 10px;
  background-color: #333;
  color: white;
}




// Simple form validation for contact form
document.getElementById('contactForm').addEventListener('submit', function (event) {
  event.preventDefault();

  let name = document.getElementById('name').value;
  let email = document.getElementById('email').value;
  let message = document.getElementById('message').value;

  if (!name || !email || !message) {
    alert('Please fill in all fields!');
  } else {
    alert('Thank you for your message!');
  }
});
