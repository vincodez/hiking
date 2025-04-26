<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ADVENTURE WEBSITE</title>
  <style>
    body {
      margin-top: 10px;
      font-family: 'Poppins', sans-serif;
      background-image: url(/25351.jpg);
      background-size: cover;
      background-repeat: no-repeat;
      color: #fff;
    }
    nav {
      display: flex;
      justify-content: space-between;
      align-content: center;
      padding: 25px 50px;
    }
    .logo {
      font-size: 28px;
      font-weight: bold;
    }
    .nav label {
      text-decoration: none;
      color: aliceblue;
      margin-left: 25px;
      border: 2px solid transparent;
      padding: 5px 10px;
      transition: border-color 0.3s;
      cursor: pointer;
      display: inline-block;
    }
    .nav label:hover {
      border-color: grey;
    }
    .hero {
      text-align: center;
      margin-top: 10%;
      padding: 0 20px;
    }
    .hero h1 {
      font-size: 80px;
      margin-top: 20px;
    }
    .hero p {
      font-size: 18px;
      max-width: 600px;
      margin: 0 auto 30px;
    }
    .btn {
      padding: 10px 30px;
      font-size: 16px;
      border-radius: 15px;
      border: none;
      background-color: #ffffffcc;
      color: #000;
      cursor: pointer;
      transition: background-color 0.3s, opacity 0.3s;
    }
    .btn:hover {
      background-color: #ffffff67;
      opacity: 0.6;
    }

    /* Hide all checkboxes */
    input[type="checkbox"] {
      display: none;
    }

    /* Common slide content style */
    .slide-content {
      position: fixed;
      top: -100%;
      left: 0;
      width: 100%;
      background: rgba(0, 0, 0, 0.9);
      color: white;
      text-align: center;
      padding: 50px 20px;
      font-size: 24px;
      transition: top 0.5s ease;
      z-index: 1000;
    }

    /* Each checkbox triggers its own slide */
    #toggle-home:checked ~ .home-slide,
    #toggle-about:checked ~ .about-slide,
    #toggle-service:checked ~ .service-slide,
    #toggle-gallery:checked ~ .gallery-slide,
    #toggle-faq:checked ~ .faq-slide,
    #toggle-contact:checked ~ .contact-slide,
    #toggle-pages:checked ~ .pages-slide {
      top: 0;
    }

    .close-btn {
      display: block;
      margin-top: 20px;
      padding: 10px 20px;
      background: white;
      color: black;
      border-radius: 8px;
      text-decoration: none;
      font-size: 16px;
      width: fit-content;
      margin-left: auto;
      margin-right: auto;
    }
    .close-btn:hover {
      background: grey;
      color: white;
    }
  </style>
</head>
<body>

  <!-- Hidden Checkboxes -->
  <input type="checkbox" id="toggle-home">
  <input type="checkbox" id="toggle-about">
  <input type="checkbox" id="toggle-service">
  <input type="checkbox" id="toggle-gallery">
  <input type="checkbox" id="toggle-faq">
  <input type="checkbox" id="toggle-contact">
  <input type="checkbox" id="toggle-pages">

  <nav>
    <div class="logo">ADVENTURE</div>
    <div class="nav">
      <label for="toggle-home">HOME</label>
      <label for="toggle-about">ABOUTUS</label>
      <label for="toggle-service">SERVICE</label>
      <label for="toggle-gallery">GALLERY</label>
      <label for="toggle-faq">FAQ</label>
      <label for="toggle-contact">CONTACTUS</label>
      <label for="toggle-pages">PAGES</label>
    </div>
  </nav>

  <div class="hero">
    <div>DISCOVER THE COLORFUL WORLD</div>
    <h1>NEW ADVENTURE</h1>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Possimus temporibus <br />
      cum commodi itaque harum, veritatis, ipsum est sint velit dolorem nobis.
    </p>
    <button class="btn">DISCOVER NOW</button>
  </div>

  <!-- Slide Contents -->

  <div class="slide-content home-slide">
    <h2>Welcome to Home Section!</h2>
    <p>This content slides down when you click "HOME".</p>
    <label for="toggle-home" class="close-btn">CLOSE</label>
  </div>

  <div class="slide-content about-slide">
    <h2>About Us</h2>
    <p>Learn more about our amazing adventures!</p>
    <label for="toggle-about" class="close-btn">CLOSE</label>
  </div>

  <div class="slide-content service-slide">
    <h2>Our Services</h2>
    <p>Explore the services we offer for your next adventure.</p>
    <label for="toggle-service" class="close-btn">CLOSE</label>
  </div>

  <div class="slide-content gallery-slide">
    <h2>Gallery</h2>
    <p>Check out the memories we've captured during our journeys!</p>
    <label for="toggle-gallery" class="close-btn">CLOSE</label>
  </div>

  <div class="slide-content faq-slide">
    <h2>FAQ</h2>
    <p>Find answers to common questions about our adventures.</p>
    <label for="toggle-faq" class="close-btn">CLOSE</label>
  </div>

  <div class="slide-content contact-slide">
    <h2>Contact Us</h2>
    <p>Get in touch and start your journey with us today!</p>
    <label for="toggle-contact" class="close-btn">CLOSE</label>
  </div>

  <div class="slide-content pages-slide">
    <h2>Pages</h2>
    <p>Explore additional pages and learn more about what we do.</p>
    <label for="toggle-pages" class="close-btn">CLOSE</label>
  </div>

</body>
</html>

