<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Residuos Informáticos</title>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>

body{
font-family: Arial, sans-serif;
margin:0;
background:#f4f7f6;
}

/* HERO */
.hero{
height:50vh;
background-image:url('residuos.jpg');
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
font-size:45px;
margin-bottom:10px;
}

.hero p{
font-size:18px;
}

/* MENÚ */
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

/* CONTENIDO */
main{
max-width:1100px;
margin:auto;
padding:20px;
}

/* TARJETAS */
.card{
background:white;
padding:25px;
margin:20px 0;
border-radius:10px;
box-shadow:0 4px 10px rgba(0,0,0,0.1);
transition:all 0.3s ease;
opacity:0;
transform:translateY(30px);
}

.card.show{
opacity:1;
transform:translateY(0);
}

.card:hover{
transform:translateY(-8px);
box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

.card h2{
margin-bottom:10px;
color:#2e8b57;
}

ul{
line-height:1.7;
}

/* FOOTER */
footer{
background:#111;
color:white;
text-align:center;
padding:20px;
margin-top:30px;
}

</style>
</head>

<body>

<div class="hero">
<div class="hero-content">
<h1>💻 Residuos Informáticos</h1>
<p>El problema de la basura electrónica</p>
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
<h2>¿Qué son los residuos informáticos?</h2>

<p>
Los residuos informáticos, también conocidos como basura electrónica o e-waste, son los dispositivos electrónicos que han sido desechados porque ya no funcionan o han quedado obsoletos.
</p>

<p>
Entre ellos se encuentran ordenadores, teléfonos móviles, impresoras, teclados, monitores y otros aparatos tecnológicos.
</p>

</section>

<section class="card">
<h2>Ejemplos de residuos informáticos</h2>

<ul>
<li>Ordenadores y portátiles antiguos.</li>
<li>Teléfonos móviles que ya no se utilizan.</li>
<li>Monitores y televisores.</li>
<li>Impresoras y escáneres.</li>
<li>Teclados, ratones y cables.</li>
</ul>

</section>

<section class="card">
<h2>Impacto en el medio ambiente</h2>

<p>
Los residuos electrónicos pueden ser muy peligrosos para el medio ambiente porque contienen materiales tóxicos como plomo, mercurio y cadmio.
</p>

<ul>
<li>Contaminación del suelo.</li>
<li>Contaminación del agua.</li>
<li>Daños en la salud de las personas.</li>
<li>Acumulación de basura tecnológica.</li>
</ul>

</section>

<section class="card">
<h2>Cómo reducir los residuos electrónicos</h2>

<ul>
<li>Reutilizar los dispositivos cuando sea posible.</li>
<li>Reparar equipos en lugar de tirarlos.</li>
<li>Donar dispositivos que todavía funcionen.</li>
<li>Reciclar los aparatos electrónicos en puntos de reciclaje.</li>
</ul>

</section>

</main>

<footer>
<p>Proyecto de Informática y Medio Ambiente</p>
<p>Autores: (Nombre del grupo)</p>
<p>2026</p>
</footer>

<script>

const observer = new IntersectionObserver(entries => {
 entries.forEach(entry => {
  if(entry.isIntersecting){
   entry.target.classList.add('show');
  }
 });
});

const elements = document.querySelectorAll('.card');
elements.forEach(el => observer.observe(el));

</script>

</body>
</html>
