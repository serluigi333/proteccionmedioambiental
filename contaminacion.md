<html lang="es">
<head>
<meta charset="UTF-8">
<title>Contaminación ambiental</title>

<!-- ESTILO INTERNO COHERENTE -->
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

/* IMÁGENES */
img{
  width:100%;
  max-width:500px;
  display:block;
  margin:auto;
  border-radius:8px;
  transition:transform 0.4s ease, box-shadow 0.4s ease;
}

img:hover{
  transform:scale(1.05);
  box-shadow:0 10px 25px rgba(0,0,0,0.3);
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

<header>
  <h1>Contaminación ambiental</h1>
  <p>Impacto de la tecnología en el medio ambiente</p>
</header>

<nav>
  <a href="index.md">Inicio</a>
  <a href="residuos.md">Residuos</a>
  <a href="obsolescencia.md">Obsolescencia</a>
  <a href="informatica-ecologica.md">Informática ecológica</a>
</nav>

<main>

<section class="card">
  <h2>¿Qué es la contaminación ambiental?</h2>
  <p>
    La contaminación ambiental es la presencia de sustancias o actividades
    que dañan el medio ambiente. Puede afectar al aire, al agua y al suelo.
    Las actividades humanas son la principal causa de este problema.
  </p>
  <img src="img/contaminacion.jpg" alt="Contaminación ambiental">
</section>

<section class="card">
  <h2>Relación con la tecnología</h2>
  <p>
    La fabricación de dispositivos electrónicos requiere minerales,
    energía y procesos industriales que generan emisiones contaminantes.
    Además, el consumo de electricidad de los dispositivos también
    contribuye al impacto ambiental.
  </p>
</section>

</main>

<footer>
  <p>Proyecto Informática Ambiental</p>
  <p>Autores: (Nombre del grupo)</p>
  <p>2026</p>
</footer>

<!-- ANIMACIÓN AL HACER SCROLL -->
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
