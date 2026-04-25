<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Imagine X</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

<style>

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Inter', sans-serif;
}

body {
  background: linear-gradient(135deg, #0a0014, #14002a);
  color: #fff;
}

/* NAV */
header {
  position: fixed;
  width: 100%;
  padding: 20px 60px;
  display: flex;
  justify-content: space-between;
  backdrop-filter: blur(10px);
  background: rgba(255,255,255,0.05);
}

.logo {
  font-weight: 600;
  font-size: 20px;
  color: #d6b3ff;
}

nav a {
  color: #ccc;
  margin-left: 25px;
  text-decoration: none;
  position: relative;
}

nav a::after {
  content: "";
  position: absolute;
  width: 0%;
  height: 2px;
  background: #b366ff;
  bottom: -5px;
  left: 0;
  transition: 0.3s;
}

nav a:hover::after {
  width: 100%;
}

/* HERO */
.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 0 60px;
}

.hero h1 {
  font-size: 70px;
  line-height: 1.1;
}

.hero span {
  color: #b366ff;
}

.hero p {
  margin-top: 15px;
  color: #aaa;
  max-width: 500px;
}

.btn {
  margin-top: 25px;
  padding: 12px 25px;
  background: #b366ff;
  border: none;
  color: #fff;
  cursor: pointer;
  border-radius: 30px;
  transition: 0.3s;
}

.btn:hover {
  transform: scale(1.05);
}

/* SECTION */
.section {
  padding: 100px 60px;
}

/* GRID */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 25px;
}

.card {
  background: rgba(255,255,255,0.05);
  border-radius: 15px;
  overflow: hidden;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-10px);
}

.card img {
  width: 100%;
}

.card p {
  padding: 15px;
}

/* ABOUT */
.about {
  max-width: 600px;
  color: #bbb;
}

/* FOOTER */
footer {
  text-align: center;
  padding: 40px;
  color: #777;
}

</style>
</head>

<body>

<header>
  <div class="logo">Imagine X</div>
  <nav>
    <a href="#home">Home</a>
    <a href="#work">Work</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero" id="home">
  <h1>Design That Feels <span>Premium</span></h1>
  <p>I craft bold and clean visuals that elevate brands and make them unforgettable.</p>
  <button class="btn">View Work</button>
</section>

<section id="work" class="section">
  <h2>Selected Work</h2>
  <div class="grid">

    <div class="card">
      <img src="https://via.placeholder.com/500">
      <p>Luxury Salon Flyer</p>
    </div>

    <div class="card">
      <img src="https://via.placeholder.com/500">
      <p>Instagram Ad Campaign</p>
    </div>

    <div class="card">
      <img src="https://via.placeholder.com/500">
      <p>Brand Identity Design</p>
    </div>

  </div>
</section>

<section id="about" class="section">
  <h2>About</h2>
  <p class="about">
    Imagine X is a creative design brand focused on delivering premium visual experiences.
    Every design is crafted with intention, clarity, and bold creativity.
  </p>
</section>

<section id="contact" class="section">
  <h2>Contact</h2>
  <p>Email: your@email.com</p>
</section>

<footer>
  © 2026 Imagine X
</footer>

</body>
</html>
