<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Profile</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #004080;
      color: white;
      padding: 20px;
      text-align: center;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      padding: 20px;
    }
    .bio {
      display: flex;
      align-items: center;
      gap: 20px;
    }
    .bio img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
    }
    footer {
      background-color: #f0f0f0;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <!-- Header with navigation -->
  <header>
    <h1>My Profile</h1>
    <nav>
      <a href="#about">About Me</a>
      <a href="#hobbies">Hobbies</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Bio section -->
  <section id="about">
    <h2>About Me</h2>
    <div class="bio">
      <img src="img/me.jpg.jpg" alt="My photo">
      <p>Hello! I'm Ahmed, a passionate and meticulous production supervisor with 5+ years of experience in processing and packaging, especially in dairy products like milk, yogurt, and juice. I love creating efficient systems and learning new things every day.</p>
    </div>
  </section>

  <!-- Hobbies section -->
  <section id="hobbies">
    <h2>My Hobbies</h2>
    <ul>
      <li>Reading leadership and motivational books</li>
      <li>Exploring new tech tools and apps</li>
      <li>Watching documentaries and local dramas</li>
    </ul>
  </section>

  <!-- Footer with contact -->
  <footer id="contact">
    <p>📧 Email: ahmed.saroke@example.com</p>
    <p>📱 Instagram: <a href="https://instagram.com/ahmed_saroke" target="_blank">@ahmed_saroke</a></p>
  </footer>

</body>
</html>
