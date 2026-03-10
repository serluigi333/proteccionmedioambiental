<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Informática y Medio Ambiente</title>

<style>

body{
font-family: Arial, sans-serif;
margin:0;
background:#f4f7f6;
}

.hero{
height:60vh;
background-image:url('img/eco.jpg');
background-size:cover;
background-position:center;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
color:white;
position:relative;
}

.hero::after{
content:"";
position:absolute;
top:0;
left:0;
right:0;
bottom:0;
background:rgba(0,0,0,0.45);
}

.hero-content{
position:relative;
z-index:1;
}

.hero h1{
font-size:48px;
margin:0;
}

.hero p{
font-size:20px;
}

nav{
background:#222;
padding:12px;
text-align:center;
}

nav a{
color:white;
margin:10px;
text-decoration:none;
font-weight:bold;
padding:8px 14px;
border-radius:6px;
transition:all 0.3s ease;
}

nav a:hover{
background:#7CFC00;
color:#000;
transform:scale(1.1);
}

main{
max-width:1000px;
margin:auto;
padding:20px;
}

.card{
background:white;
padding:25px;
margin:20px 0;
border-radius:10px;
box-shadow:0 4px 10px rgba(0,0,0,0.1);
transition:all 0.3s ease;
animation:fadein 1s;
}

.card:hover{
transform:translateY(-8px);
box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

.temas{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px;
margin-top:30px;
}

.tema{
background:white;
padding:20px;
border-radius:10px;
text-align:center;
box-shadow:0 4px 10px rgba(0,0,0,0.1);
transition:all 0.3s ease;
}

.tema:hover{
transform:scale(1.05);
box-shadow:0 10px 20px rgba(0,0,0,0.2);
}

.icono{
font-size:40px;
margin-bottom:10px;
}

footer{
background:#111;
color:white;
text-align:center;
padding:20px;
margin-top:30px;
}

@keyframes fadein{
from{opacity:0; transform:translateY(20px);} 
to{opacity:1; transform:translateY(0);} 
}

</style>

</head>

<body>

<div class="hero">
<div class="hero-content">
<h1>🌍 Informática y Protección Medioambiental</h1>
<p>Cómo la tecnología afecta al planeta</p>
</div>
</div>

<nav>
<a href="index.html">Inicio</a>
<a href="contaminacion.html">Contaminación</a>
<a href="residuos.html">Residuos informáticos</a>
<a href="obsolescencia.html">Obsolescencia</a>
<a href="informatica-ecologica.html">Informática ecológica</a>
<a href="referencias.html">Referencias</a>
</nav>

<main>

<section class="card">
<h2>Introducción</h2>
<p>La informática forma parte de nuestra vida diaria. Utilizamos ordenadores, teléfonos móviles y muchos dispositivos electrónicos para trabajar, estudiar y comunicarnos. Sin embargo, la producción y el uso de estos dispositivos puede generar contaminación y residuos tecnológicos.</p>
<p>Este proyecto analiza el impacto de la tecnología en el medio ambiente y muestra posibles soluciones para un uso más sostenible.</p>
</section>

<section class="card">
<h2>Temas del proyecto</h2>

<div class="temas">

<div class="tema">
<div class="icono">🏭</div>
<h3>Contaminación ambiental</h3>
<p>Impacto de las actividades humanas y tecnológicas en el medio ambiente.</p>
</div>

<div class="tema">
<div class="icono">💻</div>
<h3>Residuos informáticos</h3>
<p>Dispositivos electrónicos que se desechan y generan contaminación.</p>
</div>

<div class="tema">
<div class="icono">⏳</div>
<h3>Obsolescencia programada</h3>
<p>Productos diseñados para durar menos tiempo y fomentar el consumo.</p>
</div>

<div class="tema">
<div class="icono">🌱</div>
<h3>Informática ecológica</h3>
<p>Uso de tecnología eficiente y sostenible para reducir el impacto ambiental.</p>
</div>

</div>

</section>

</main>

<footer>
<p>Proyecto educativo de informática</p>
<p>Autores: (Nombre del grupo)</p>
<p>2026</p>
</footer>

</body>
</html>
