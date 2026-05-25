# velvetrootsstudio
Estudio webcam 
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Velvet Roots Studio</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Cormorant+Garamond:wght@300;400;500&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#070707;
    color:#f5e7e7;
    font-family:'Cormorant Garamond', serif;
    overflow-x:hidden;
}

body::before{
    content:"";
    position:fixed;
    inset:0;
    background:
    radial-gradient(circle at top left, rgba(90,30,43,.25), transparent 35%),
    radial-gradient(circle at bottom right, rgba(198,165,107,.08), transparent 35%);
    z-index:-1;
}

header{
    position:fixed;
    top:0;
    width:100%;
    padding:20px 8%;
    backdrop-filter:blur(10px);
    background:rgba(0,0,0,.45);
    border-bottom:1px solid rgba(255,255,255,.05);
    z-index:1000;
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-family:'Playfair Display', serif;
    color:#d4b08c;
    font-size:28px;
    letter-spacing:2px;
}

.menu{
    display:flex;
    gap:30px;
}

.menu a{
    text-decoration:none;
    color:#f5dede;
    transition:.3s;
    font-size:18px;
}

.menu a:hover{
    color:#d4b08c;
}

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    text-align:center;
    padding:140px 10%;
}

.hero img{
    width:340px;
    max-width:90%;
    margin-bottom:40px;
    border-radius:20px;
    box-shadow:0 0 40px rgba(212,176,140,.15);
}

.hero h1{
    font-size:70px;
    font-family:'Playfair Display', serif;
    color:#d4b08c;
    margin-bottom:25px;
}

.hero p{
    max-width:850px;
    font-size:28px;
    line-height:1.7;
    color:#e8d3d3;
}

.buttons{
    margin-top:45px;
    display:flex;
    gap:20px;
    flex-wrap:wrap;
    justify-content:center;
}

.btn{
    padding:15px 35px;
    border-radius:40px;
    text-decoration:none;
    font-size:18px;
    transition:.4s;
}

.btn-primary{
    background:#5a1e2b;
    color:white;
}

.btn-primary:hover{
    background:#7a3041;
}

.btn-secondary{
    border:1px solid #d4b08c;
    color:#d4b08c;
}

.btn-secondary:hover{
    background:#d4b08c;
    color:black;
}

section{
    padding:120px 10%;
}

.section-title{
    text-align:center;
    margin-bottom:70px;
}

.section-title h2{
    font-size:52px;
    font-family:'Playfair Display', serif;
    color:#d4b08c;
    margin-bottom:15px;
}

.section-title p{
    font-size:22px;
    color:#d9c3c3;
}

.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
    gap:30px;
}

.card{
    background:rgba(255,255,255,.03);
    padding:40px;
    border-radius:24px;
    border:1px solid rgba(255,255,255,.05);
    transition:.4s;
}

.card:hover{
    transform:translateY(-8px);
    border-color:#5a1e2b;
}

.card h3{
    color:#d4b08c;
    font-size:30px;
    margin-bottom:20px;
    font-family:'Playfair Display', serif;
}

.card p,
.card li{
    font-size:22px;
    line-height:1.8;
    color:#f0dddd;
}

.card ul{
    padding-left:20px;
}

.join{
    text-align:center;
}

.join-box{
    max-width:900px;
    margin:auto;
    background:linear-gradient(145deg,#111,#1b0e12);
    padding:60px;
    border-radius:30px;
    border:1px solid rgba(212,176,140,.1);
}

.join-box h2{
    font-size:52px;
    color:#d4b08c;
    margin-bottom:25px;
    font-family:'Playfair Display', serif;
}

.join-box p{
    font-size:24px;
    line-height:1.8;
}

.process{
    margin-top:40px;
    text-align:left;
}

.process li{
    margin-bottom:15px;
    font-size:22px;
}

.notice{
    background:#13090c;
    text-align:center;
}

.notice h2{
    color:#d4b08c;
    margin-bottom:20px;
    font-size:44px;
}

.notice p{
    font-size:24px;
    max-width:900px;
    margin:auto;
    line-height:1.8;
}

.contact{
    text-align:center;
}

.contact p{
    font-size:24px;
    margin-bottom:15px;
}

footer{
    padding:60px 10%;
    text-align:center;
    border-top:1px solid rgba(255,255,255,.05);
    background:black;
}

footer p{
    color:#bfa5a5;
    margin-bottom:12px;
    font-size:18px;
}

@media(max-width:768px){

.hero h1{
    font-size:42px;
}

.hero p{
    font-size:22px;
}

.section-title h2{
    font-size:38px;
}

.menu{
    gap:15px;
    font-size:15px;
}

.card p,
.card li{
    font-size:20px;
}

}

</style>
</head>

<body>

<header>

<nav>

<div class="logo">
Velvet Roots Studio
</div>

<div class="menu">
<a href="#inicio">Inicio</a>
<a href="#nosotras">Nosotras</a>
<a href="#servicios">Servicios</a>
<a href="#unete">Únete</a>
<a href="#contacto">Contacto</a>
</div>

</nav>

</header>

<section class="hero" id="inicio">

<img src="logo.jpeg" alt="Velvet Roots Studio">

<h1>
Elegancia. Profesionalismo. Confidencialidad.
</h1>

<p>
Estudio webcam boutique en Barcelona especializado en contenido adulto premium +18 para plataformas internacionales.
</p>

<div class="buttons">

<a href="#unete" class="btn btn-primary">
Únete al Studio
</a>

<a href="#contacto" class="btn btn-secondary">
Contacto Privado
</a>

</div>

</section>

<section id="nosotras">

<div class="section-title">
<h2>🖤 Bienvenida</h2>
<p>
Un entorno seguro, elegante y confidencial.
</p>
</div>

<div class="grid">

<div class="card">

<h3>Velvet Roots Studio</h3>

<p>
Velvet Roots Studio es un estudio webcam profesional ubicado en Barcelona, especializado en transmisiones para plataformas internacionales como Stripchat, Chaturbate y BongaCams.
</p>

</div>

<div class="card">

<h3>🌹 Filosofía</h3>

<ul>
<li>✨ Entorno seguro y privado</li>
<li>💼 Gestión profesional y transparente</li>
<li>📈 Formación y estrategia</li>
<li>💰 Distribución justa</li>
<li>🔒 Confidencialidad absoluta</li>
<li>🌍 Alcance internacional</li>
</ul>

</div>

</div>

</section>

<section id="servicios">

<div class="section-title">
<h2>👑 Servicios</h2>
<p>
Servicios premium para modelos y colaboraciones.
</p>
</div>

<div class="grid">

<div class="card">

<h3>Para Modelos</h3>

<ul>
<li>Formación profesional</li>
<li>Asesoría de imagen</li>
<li>Producción audiovisual</li>
<li>Soporte técnico en vivo</li>
<li>Espacios privados premium</li>
<li>Asesoría fiscal y legal</li>
<li>Protección de identidad</li>
</ul>

</div>

<div class="card">

<h3>Para Colaboraciones</h3>

<ul>
<li>Producción audiovisual discreta</li>
<li>Consultoría de marca</li>
<li>Redes sociales</li>
<li>Identidad visual</li>
<li>Promoción estratégica</li>
</ul>

</div>

</div>

</section>

<section class="join" id="unete">

<div class="join-box">

<h2>
💼 Únete a Velvet Roots Studio
</h2>

<p>
Buscamos mujeres mayores de edad interesadas en trabajar en un entorno profesional, ético y rentable.
</p>

<ol class="process">
<li>Enviar solicitud</li>
<li>Entrevista privada</li>
<li>Firma NDA</li>
<li>Formación inicial</li>
<li>Inicio de transmisiones</li>
</ol>

<div class="buttons">

<a href="mailto:velvetrootsstudio@gmail.com" class="btn btn-primary">
Aplicar Ahora
</a>

</div>

</div>

</section>

<section class="notice">

<h2>⚠️ Aviso +18</h2>

<p>
Este sitio contiene información y material destinado exclusivamente a personas mayores de 18 años.
Al ingresar, confirmas ser mayor de edad y que el acceso a este contenido es legal en tu país.
</p>

</section>

<section class="contact" id="contacto">

<div class="section-title">
<h2>📧 Contacto</h2>
<p>
Barcelona, España
</p>
</div>

<p>
velvetrootsstudio@gmail.com
</p>

<p>
Instagram: @velvetroots.studio
</p>

<p>
Twitter/X: @velvetroots_es
</p>

</section>

<footer>

<p>
© 2026 Velvet Roots Studio – Todos los derechos reservados
</p>

<p>
Estudio Webcam Profesional | Barcelona, España
</p>

<p>
+18 | Acceso exclusivo para adultos
</p>

</footer>

</body>
</html>
