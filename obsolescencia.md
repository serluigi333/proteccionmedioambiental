<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Obsolescencia Programada</title>

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
background-image:url('obsolescencia.jpg');
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

/* MENU */
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

/* LISTAS */
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
<h1>⏳ Obsolescencia Programada</h1>
<p>Cuando la tecnología está diseñada para durar menos</p>
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
<h2>¿Qué es la obsolescencia programada?</h2>

<p>
La obsolescencia programada es una estrategia utilizada por algunas empresas para diseñar productos con una vida útil limitada.
Esto significa que los dispositivos dejan de funcionar correctamente o se vuelven obsoletos después de cierto tiempo.
</p>

<p>
En el ámbito de la informática y la tecnología esto ocurre con ordenadores, teléfonos móviles, impresoras y otros dispositivos electrónicos.
</p>

</section>

<section class="card">
<h2>Tipos de obsolescencia</h2>

<ul>
<li><strong>Obsolescencia técnica:</strong> el dispositivo deja de funcionar por fallos o desgaste.</li>

<li><strong>Obsolescencia de software:</strong> los programas o sistemas dejan de recibir actualizaciones.</li>

<li><strong>Obsolescencia psicológica:</strong> los consumidores cambian de producto porque aparece uno más moderno.</li>
</ul>

</section>

<section class="card">
<h2>Consecuencias para el medio ambiente</h2>

<p>
La obsolescencia programada tiene un impacto negativo en el medio ambiente porque provoca un aumento del consumo y de los residuos electrónicos.
</p>

<ul>
<li>Mayor cantidad de basura tecnológica.</li>
<li>Uso excesivo de recursos naturales.</li>
<li>Contaminación por materiales tóxicos.</li>
<li>Mayor gasto energético en la fabricación de nuevos dispositivos.</li>
</ul>

</section>

<section class="card">
<h2>¿Cómo podemos reducirla?</h2>

<ul>
<li>Reparar los dispositivos en lugar de reemplazarlos.</li>
<li>Comprar productos de mayor calidad y duración.</li>
<li>Actualizar software cuando sea posible.</li>
<li>Reciclar correctamente los dispositivos electrónicos.</li>
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
