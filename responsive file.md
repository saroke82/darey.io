<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Welcome - Landing Page</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      line-height: 1.6;
      background-color: #f5f8fc;
      color: #333;
    }

    header {
      background-color: #004080;
      color: white;
      padding: 20px;
    }

    .nav-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      max-width: 1200px;
      margin: auto;
    }

    .logo {
      font-size: 24px;
      font-weight: bold;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }

    nav {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }

    .hero {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 80vh;
      text-align: center;
      background: linear-gradient(to right, #0066cc, #003366);
      color: white;
      padding: 20px;
    }

    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 15px;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 25px;
    }

    .btn {
      padding: 12px 25px;
      background-color: white;
      color: #004080;
      font-weight: bold;
      text-decoration: none;
      border-radius: 5px;
      transition: background 0.3s ease;
    }

    .btn:hover {
      background-color: #e0e0e0;
    }

    footer {
      background-color: #f0f0f0;
      padding: 20px;
      text-align: center;
      font-size: 0.9rem;
    }

    /* Responsive styles */
    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2rem;
      }

      nav {
        flex-direction: column;
        margin-top: 10px;
      }

      nav a {
        margin: 5px 0;
      }
    }
  </style>
</head>
<body>

  <!-- Header with navigation -->
  <header>
    <div class="nav-container">
      <div class="logo">MyBrand</div>
      <nav>
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <h1>Welcome to My World</h1>
    <p>Your one-stop spot for everything creative, smart and impactful.</p>
    <a href="#contact" class="btn">Get in Touch</a>
  </section>

  <!-- Footer -->
  <footer id="contact">
    <p>Contact me: ahmed.saroke@example.com | IG: @ahmed_saroke</p>
  </footer>

</body>
</html>
