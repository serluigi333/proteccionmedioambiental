<!DOCTYPE html>

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

/* HEADER */

header{
background:linear-gradient(135deg,#2e8b57,#3cb371);
color:white;
padding:40px;
text-align:center;
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

/* EFECTO HOVER EN MENÚ */

nav a:hover{
background:#7CFC00;
color:#000;
transform:scale(1.1);
}

/* CONTENIDO */

main{
max-width:1000px;
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
}

/* EFECTO HOVER TARJETAS */

.card:hover{
transform:translateY(-8px);
box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

/* IMÁGENES */

img{
width:100%;
max-width:500px;
display:block;
margin:auto;
border-radius:8px;
transition:transform 0.4s ease, box-shadow 0.4s ease;
}

/* EFECTO HOVER IMÁGENES */

img:hover{
transform:scale(1.05);
box-shadow:0 10px 25px rgba(0,0,0,0.3);
}

/* BOTONES */

button{
background:#2e8b57;
color:white;
border:none;
padding:12px 20px;
border-radius:6px;
cursor:pointer;
font-size:16px;
transition:all 0.3s ease;
}

button:hover{
background:#3cb371;
transform:scale(1.1);
}

/* FOOTER */

footer{
background:#111;
color:white;
text-align:center;
padding:20px;
margin-top:30px;
}

/* ANIMACIÓN AL CARGAR */

@keyframes fadein{
from{opacity:0; transform:translateY(20px);}
to{opacity:1; transform:translateY(0);}
}

.card{
animation:fadein 1s;
}

</style>

</head>

<body>

<header>
<h1>🌍 Informática y Protección Medioambiental</h1>
<p>El impacto de la tecnología en el planeta</p>
</header>

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

<p>
La informática forma parte de nuestra vida diaria. Utilizamos ordenadores,
teléfonos móviles, tablets y muchos otros dispositivos para trabajar,
estudiar y comunicarnos.
</p>

<p>
Sin embargo, la producción de estos dispositivos requiere recursos
naturales, energía y procesos industriales que pueden generar contaminación
y residuos electrónicos. Por esta razón es importante analizar cómo la
tecnología afecta al medio ambiente.
</p>

<img src="img/eco.jpg" alt="Tecnología sostenible">

</section>

<section class="card">

<h2>Objetivo del proyecto</h2>

<ul>
<li>Comprender qué es la contaminación ambiental</li>
<li>Analizar el problema de los residuos electrónicos</li>
<li>Explicar la obsolescencia programada</li>
<li>Conocer qué es la informática ecológica</li>
</ul>

</section>

<section class="card">

<h2>¿Por qué es importante?</h2>

<p>
El uso responsable de la tecnología puede ayudar a reducir el impacto
ambiental. Reciclar dispositivos, alargar su vida útil y utilizar
equipos eficientes energéticamente son algunas de las medidas que
contribuyen a proteger el medio ambiente.
</p>

<button>Más información</button>

</section>

</main>

<footer>

<p>Proyecto educativo de informática</p>
<p>Autores: (Nombre del grupo)</p>
<p>2026</p>

</footer>

</body>
</html>
