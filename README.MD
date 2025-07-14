<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Edit by Bhawan</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #fff;
      color: #222;
    }
    header {
      background: #f4f4f4;
      padding: 40px;
      text-align: center;
    }
    header img {
      max-width: 200px;
      border-radius: 16px;
    }
    h1 {
      margin-top: 20px;
      font-size: 2.5rem;
    }
    section {
      padding: 40px 20px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .grid img, .grid video {
      width: 100%;
      border-radius: 12px;
    }
    footer {
      background: #222;
      color: white;
      padding: 30px;
      text-align: center;
    }
    a {
      color: #0077cc;
      text-decoration: none;
    }
    .tools {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
    }
    .tools span {
      background: #eee;
      padding: 8px 14px;
      border-radius: 20px;
      font-weight: bold;
    }
    .button {
      background: #25D366;
      color: white;
      padding: 12px 20px;
      border-radius: 8px;
      display: inline-block;
      margin-top: 10px;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <!-- HERO SECTION -->
  <header>
    <img src="your-image.jpg" alt="Bhawan Main">
    <h1>Welcome to Edit by Bhawan</h1>
  </header>

  <!-- ANIMATION PROJECTS -->
  <section>
    <h2>Animation Projects</h2>
    <div class="grid">
      <img src="project1.jpg" alt="Animation 1">
      <img src="project2.jpg" alt="Animation 2">
      <img src="project3.jpg" alt="Animation 3">
    </div>
  </section>

  <!-- YOUTUBE EDITS -->
  <section>
    <h2>YouTube Edits</h2>
    <div class="grid">
      <video controls>
        <source src="edit1.mp4" type="video/mp4">
      </video>
      <video controls>
        <source src="edit2.mp4" type="video/mp4">
      </video>
    </div>
  </section>

  <!-- WEDDING EDITS -->
  <section>
    <h2>Wedding Edits</h2>
    <div class="grid">
      <img src="wedding1.jpg" alt="Wedding 1">
      <img src="wedding2.jpg" alt="Wedding 2">
    </div>
  </section>

  <!-- TOOLS I USE -->
  <section>
    <h2>Tools I Use</h2>
    <div class="tools">
      <span>Adobe Premiere Pro</span>
      <span>Adobe Animate</span>
      <span>After Effects</span>
      <span>Illustrator</span>
      <span>Blender</span>
    </div>
  </section>

  <!-- BOOK YOUR EDIT -->
  <section>
    <h2>Book Your Edit</h2>
    <p>
      Want to work together? Let’s connect on WhatsApp or Razorpay:
    </p>
    <a class="button" href="https://wa.me/yourwhatsapplink" target="_blank">
      📱 WhatsApp Me
    </a>
    <br>
    <a class="button" href="https://razorpay.me/yourpaymentlink" target="_blank" style="background:#6366F1">
      💳 Pay on Razorpay
    </a>
  </section>

  <!-- CONTACT -->
  <footer>
    <p>Contact me at: <a href="mailto:youremail@example.com">youremail@example.com</a></p>
    <p>Behance: 
      <a href="https://www.behance.net/yourbehanceusername" target="_blank">
        behance.net/yourbehanceusername
      </a>
    </p>
    <p>WhatsApp: <a href="https://wa.me/yourwhatsapplink" target="_blank">Chat Now</a></p>
  </footer>

</body>
</html>
