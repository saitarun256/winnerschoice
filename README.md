# winnerschoice
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Winners Choice</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Montserrat', sans-serif;
      background: linear-gradient(to right, #f0f2f5, #e0eafc);
      color: #333;
      line-height: 1.6;
    }

    header {
      background: #0d47a1;
      color: white;
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 2px 10px rgba(0,0,0,0.2);
    }

    header h1 {
      font-size: 3em;
      font-weight: 800;
      letter-spacing: 1px;
      animation: fadeInDown 1s ease-out;
    }

    .container {
      max-width: 1100px;
      margin: 40px auto;
      padding: 20px;
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.1);
      animation: fadeInUp 1s ease-in;
    }

    .quote {
      font-size: 1.8em;
      font-weight: 600;
      text-align: center;
      color: #0d47a1;
      margin: 30px 0;
      transition: 0.3s;
    }

    .quote:hover {
      color: #0b3861;
    }

    h2.join {
      text-align: center;
      font-size: 2.5em;
      color: #0d47a1;
      margin-top: 50px;
      animation: pulse 2s infinite;
    }

    p {
      font-size: 1.1em;
      margin: 20px 0;
      color: #444;
    }

    form {
      margin-top: 30px;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    input, textarea {
      padding: 14px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 1em;
      transition: border 0.3s;
    }

    input:focus, textarea:focus {
      border: 1px solid #0d47a1;
      outline: none;
    }

    button {
      background: #0d47a1;
      color: white;
      border: none;
      padding: 14px;
      font-size: 1em;
      font-weight: 600;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background: #093371;
    }

    @keyframes fadeInDown {
      from {
        opacity: 0;
        transform: translateY(-20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes pulse {
      0%, 100% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.03);
      }
    }

    @media (max-width: 768px) {
      .quote {
        font-size: 1.4em;
      }

      h2.join {
        font-size: 2em;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Winners Choice</h1>
  </header>

  <div class="container">
    <div class="quote">
      "Passive income is the path to freedom—build systems that work for you."
    </div>

    <p>
      Welcome to the Winners Choice program—an innovative journey where we guide you in building sustainable, automated income. Through expert strategies, real-world tools, and community mentorship, you'll learn how to invest time wisely today to earn continuously tomorrow. From affiliate marketing to digital investments, we’ve got you covered.
    </p>

    <h2 class="join">Let's Join in This Program</h2>

    <p>
      Your tasks include content sharing, referral building, completing learning modules, and promoting your growth journey through our platform. These activities not only teach you valuable digital skills but also generate continuous rewards. Our support team and mentors are ready to help you get started today!
    </p>

    <form id="contactForm">
      <input type="text" id="name" placeholder="Your Name" required />
      <input type="tel" id="mobile" placeholder="Mobile Number" required />
      <input type="email" id="email" placeholder="Email Address" required />
      <textarea id="message" placeholder="Your Message" rows="5" required></textarea>
      <button type="submit">Contact With Us</button>
    </form>
  </div>

  <script>
    document.getElementById("contactForm").addEventListener("submit", function(e) {
      e.preventDefault();
      const name = document.getElementById("name").value;
      alert(`Thank you, ${name}. We'll contact you shortly!`);

      // Optional: Send data to server or integrate with email service
    });
  </script>

</body>
</html>
