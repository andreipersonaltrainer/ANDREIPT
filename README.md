<!DOCTYPE html>
<html lang="ro">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ANDREIPT | Personal Trainer</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    * {margin:0; padding:0; box-sizing:border-box;}
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #0d0d0d;
      color: #fff;
      line-height: 1.6;
    }
    header {
      display:flex; justify-content:space-between; align-items:center;
      padding:20px 60px; background:#111; position:sticky; top:0; z-index:1000;
    }
    header img {height:60px;}
    nav a {
      color:#fff; text-decoration:none; margin:0 15px; font-weight:500;
      transition: color 0.3s;
    }
    nav a:hover {color:#00bcd4;}
    section {padding:80px 60px;}
    .hero {
      display:flex; flex-direction:column; align-items:center; justify-content:center;
      text-align:center; height:90vh;
      background: linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?auto=format&fit=crop&w=1400&q=60') center/cover;
    }
    .hero h1 {font-size:3rem; margin-bottom:20px;}
    .hero p {font-size:1.2rem; margin-bottom:30px;}
    .btn {
      background:#00bcd4; color:#fff; padding:12px 25px; border:none;
      border-radius:5px; cursor:pointer; text-transform:uppercase; letter-spacing:1px;
      transition:background 0.3s;
    }
    .btn:hover {background:#0193a5;}
    h2 {text-align:center; font-size:2rem; margin-bottom:40px;}
    .services, .products {
      display:grid; grid-template-columns:repeat(auto-fit, minmax(250px,1fr)); gap:30px;
    }
    .card {
      background:#1a1a1a; padding:20px; border-radius:10px; text-align:center;
      transition:transform 0.3s, background 0.3s;
    }
    .card:hover {transform:translateY(-5px); background:#222;}
    .card img {width:100%; border-radius:10px; margin-bottom:15px;}
    footer {
      background:#111; text-align:center; padding:30px; margin-top:40px;
    }
    form {max-width:500px; margin:0 auto;}
    input, textarea {
      width:100%; padding:10px; margin:10px 0; border:none; border-radius:5px;
      background:#222; color:#fff;
    }
    input[type="submit"] {
      background:#00bcd4; cursor:pointer; font-weight:bold;
    }
    input[type="submit"]:hover {background:#0193a5;}
  </style>
</head>
<body>

  <header>
    <img src="LOGOGOOO.png" alt="ANDREIPT Logo">
    <nav>
      <a href="#home">Acasă</a>
      <a href="#about">Despre mine</a>
      <a href="#services">Servicii</a>
      <a href="#shop">Magazin</a>
      <a href="#testimonials">Testimoniale</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>ANDREIPT</h1>
    <p>Transformă-ți corpul. Schimbă-ți viața.</p>
    <button class="btn" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'});">Începe acum</button>
  </section>

  <section id="about">
    <h2>Despre mine</h2>
    <p style="max-width:800px; margin:20px auto; text-align:center;">
      Sunt Andrei, antrenor personal dedicat să te ajut să-ți atingi obiectivele de fitness prin planuri eficiente și susținere constantă.
      Cu experiență în antrenamente funcționale și nutriție, ofer programe personalizate adaptate nevoilor tale.
    </p>
  </section>

  <section id="services">
    <h2>Servicii</h2>
    <div class="services">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1517964109270-9034a21d06d3?auto=format&fit=crop&w=800&q=60" alt="">
        <h3>Antrenamente 1:1</h3>
        <p>Ședințe individuale dedicate obiectivelor tale, cu monitorizare și feedback personalizat.</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1599058917212-d750089bc07a?auto=format&fit=crop&w=800&q=60" alt="">
        <h3>Planuri Online</h3>
        <p>Programe de antrenament și nutriție trimise digital, cu suport săptămânal prin e-mail.</p>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1579758629938-03607ccdbaba?auto=format&fit=crop&w=800&q=60" alt="">
        <h3>Consultanță Nutrițională</h3>
        <p>Îmbunătățește-ți stilul de viață printr-un plan alimentar adaptat metabolismului tău.</p>
      </div>
    </div>
  </section>

  <section id="shop">
    <h2>Magazin</h2>
    <div class="products">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1523381210434-271e8be1f52b?auto=format&fit=crop&w=800&q=60" alt="">
        <h3>Tricou ANDREIPT</h3>
        <p>Material premium, design minimalist.</p>
        <button class="btn" onclick="window.open('https://www.paypal.com/demo','_blank')">Cumpără acum</button>
      </div>
      <div class="card">
        <img src="https://images.unsplash.com/photo-1605296867304-46d5465a13f1?auto=format&fit=crop&w=800&q=60" alt="">
        <h3>Plan de Antrenament (PDF)</h3>
        <p>Plan complet de 4 săptămâni, personalizabil.</p>
        <button class="btn" onclick="window.open('https://www.paypal.com/demo','_blank')">Cumpără acum</button>
      </div>
    </div>
  </section>

  <section id="testimonials">
    <h2>Testimoniale</h2>
    <p style="text-align:center; max-width:700px; margin:0 auto;">
      “Andrei m-a ajutat să-mi ating obiectivele mai repede decât credeam posibil! Recomand cu încredere.”
      <br>– Client mulțumit
    </p>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <form action="mailto:andreipersonaltrainer@yahoo.com" method="post" enctype="text/plain">
      <input type="text" name="name" placeholder="Nume" required>
      <input type="email" name="email" placeholder="Email" required>
      <textarea name="message" rows="5" placeholder="Mesajul tău..." required></textarea>
      <input type="submit" value="Trimite mesajul">
    </form>
  </section>

  <footer>
    <p>© 2025 ANDREIPT. Toate drepturile rezervate.</p>
  </footer>

</body>
</html>
