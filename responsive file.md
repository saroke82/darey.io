<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Landing Page</title>
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
      background-color: #f8f9fc;
      color: #333;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(to right, #4a90e2, #1455a3);
      color: white;
      padding: 60px 20px;
      text-align: center;
    }

    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 15px;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 25px;
      max-width: 600px;
      margin-inline: auto;
    }

    .cta-button {
      background-color: white;
      color: #1455a3;
      padding: 12px 25px;
      font-weight: bold;
      border-radius: 5px;
      display: inline-block;
      transition: background 0.3s;
    }

    .cta-button:hover {
      background-color: #f0f0f0;
    }

    /* Features Section */
    .features {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 60px 20px;
      background-color: #ffffff;
    }

    .feature {
      flex: 1 1 300px;
      max-width: 300px;
      margin: 15px;
      background: #f5f7fa;
      border-radius: 10px;
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    }

    .feature img {
      width: 50px;
      margin-bottom: 15px;
    }

    .feature h3 {
      margin-bottom: 10px;
      color: #1455a3;
    }

    /* Footer */
    footer {
      background-color: #1a1a1a;
      color: white;
      padding: 30px 20px;
      text-align: center;
    }

    footer p, footer a {
      font-size: 0.95rem;
      color: #ccc;
      margin: 5px 0;
    }

    footer a:hover {
      color: #fff;
    }

    /* Responsive Headline Size */
    @media (max-width: 600px) {
      .hero h1 {
        font-size: 2rem;
      }

      .hero p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Discover Your Perfect Workflow</h1>
    <p>Our tool helps you streamline tasks, boost productivity, and save time — all in one smart platform.</p>
    <a href="#signup" class="cta-button">Sign Up</a>
  </section>

  <!-- Features Section -->
  <section class="features">
    <div class="feature">
      <img src="https://img.icons8.com/ios-filled/50/4a90e2/lightning-bolt.png" alt="Fast">
      <h3>Fast & Efficient</h3>
      <p>Speed up your daily tasks with our intuitive automation tools and blazing-fast interface.</p>
    </div>
    <div class="feature">
      <img src="https://img.icons8.com/ios-filled/50/4a90e2/cloud.png" alt="Cloud">
      <h3>Cloud-Based</h3>
      <p>Access your data anywhere, anytime. All your work is saved securely in the cloud.</p>
    </div>
    <div class="feature">
      <img src="https://img.icons8.com/ios-filled/50/4a90e2/lock--v1.png" alt="Secure">
      <h3>Secure & Private</h3>
      <p>Built with strong encryption and privacy-first design to keep your data safe.</p>
    </div>
  </section>

  <!-- Footer Section -->
  <footer>
    <p>📧 Email: support@example.com</p>
    <p>📞 Phone: +234-801-234-5678</p>
    <p>🔗 Follow us: <a href="https://instagram.com/yourbrand" target="_blank">@yourbrand</a></p>
    <p>© 2025 YourBrand. All rights reserved.</p>
  </footer>

</body>
</html>
