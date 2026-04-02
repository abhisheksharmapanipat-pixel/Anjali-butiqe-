# Anjali-butiqe-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Anjali’s Butiq</title>

<!-- Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Poppins&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}

body{
    background:#fff;
    color:#333;
}

/* NAV */
nav{
    position:fixed;
    top:0;
    width:100%;
    background:#fff;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:10px 20px;
    box-shadow:0 2px 10px rgba(0,0,0,0.1);
    z-index:999;
}

.logo-text{
    font-family:'Playfair Display',serif;
    font-size:22px;
    font-weight:bold;
}

.tagline{
    font-size:12px;
    color:#777;
}

/* Rotating Logo */
.logo-img{
    width:50px;
    height:50px;
    border-radius:50%;
    animation:rotate 6s linear infinite;
}

@keyframes rotate{
    from{transform:rotate(0deg);}
    to{transform:rotate(360deg);}
}

/* HERO */
.hero{
    height:100vh;
    background-size:cover;
    background-position:center;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:white;
    position:relative;
}

.hero::after{
    content:'';
    position:absolute;
    width:100%;
    height:100%;
    background:rgba(0,0,0,0.4);
}

.hero-content{
    position:relative;
    z-index:1;
}

.hero h1{
    font-size:40px;
    margin-bottom:20px;
}

.btn{
    padding:12px 25px;
    background:#ff4081;
    color:#fff;
    border:none;
    cursor:pointer;
    font-size:18px;
    border-radius:30px;
}

.btn:hover{
    background:#e73370;
}

/* SERVICES */
.services{
    padding:60px 20px;
    text-align:center;
}

.carousel{
    display:flex;
    overflow-x:auto;
    gap:20px;
    padding:20px;
}

.card{
    min-width:250px;
    border-radius:15px;
    overflow:hidden;
    box-shadow:0 4px 10px rgba(0,0,0,0.1);
    background:#fff;
}

.card img{
    width:100%;
    height:200px;
    object-fit:cover;
}

.card h3{
    padding:10px;
}

.card p{
    color:#ff4081;
    font-weight:bold;
    padding-bottom:10px;
}

/* FOOTER */
footer{
    text-align:center;
    padding:20px;
    background:#111;
    color:#fff;
}

footer a{
    color:#ff4081;
}
</style>
</head>

<body>

<!-- NAVBAR -->
<nav>
<div>
<div class="logo-text">Anjali’s Butiq</div>
<div class="tagline">We offer all types of female wear stitch at very low price in market</div>
</div>
<img src="https://i.ibb.co/5g7XvmjH/IMG-3412.png" class="logo-img">
</nav>

<!-- HERO -->
<section class="hero" id="hero">
<div class="hero-content">
<h1>Welcome to Anjali’s Butiq</h1>
<button class="btn" onclick="scrollToServices()">Shop Now</button>
</div>
</section>

<!-- SERVICES -->
<section class="services" id="services">
<h2>Our Services</h2>

<div class="carousel">

<div class="card">
<img src="https://i.ibb.co/cS6pcV4h/IMG-3413.jpg">
<h3>Suit Salwar Stitch</h3>
<p>₹400</p>
</div>

<div class="card">
<img src="https://i.ibb.co/KxM3ZRPq/IMG-3414.jpg">
<h3>Plazo Stitch</h3>
<p>₹299</p>
</div>

<div class="card">
<img src="https://i.ibb.co/v6m3CMfh/IMG-3415.jpg">
<h3>Kurti Stitch</h3>
<p>₹350</p>
</div>

</div>

<br>

<a href="https://wa.me/9050953173">
<button class="btn">Order on WhatsApp</button>
</a>

</section>

<!-- FOOTER -->
<footer>
<p>Contact: <a href="mailto:abhisheksharma73031@gmail.com">abhisheksharma73031@gmail.com</a></p>
<p>THANKS FOR VISITING ❤️ LOVE FROM ANJALI’s BUTIQ</p>
</footer>

<script>

/* HERO SLIDESHOW */
const images = [
"https://i.ibb.co/xKSQXd2j/IMG-2704.jpg",
"https://i.ibb.co/fzmJtPKb/IMG-2710.jpg"
];

let index = 0;

function changeHero(){
document.querySelector('.hero').style.backgroundImage = `url(${images[index]})`;
index = (index + 1) % images.length;
}

setInterval(changeHero,3000);
changeHero();

/* SCROLL */
function scrollToServices(){
document.getElementById('services').scrollIntoView({behavior:'smooth'});
}

</script>

</body>
</html>
