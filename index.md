<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Informática y Medio Ambiente</title>

<!-- ICONOS PROFESIONALES -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: #f4f7f6;
  display: flex;
}

/* SIDEBAR LATERAL */
.sidebar {
  width: 220px;
  background: #222;
  color: white;
  position: fixed;
  top: 0;
  bottom: 0;
  padding: 20px 10px;
  overflow-y: auto;
}

.sidebar h2 {
  font-size: 20px;
  margin-bottom: 20px;
  text-align: center;
  color: #7CFC00;
}

.sidebar a {
  display: block;
  color: white;
  text-decoration: none;
  padding: 10px 15px;
  margin: 5px 0;
  border-radius: 6px;
  transition: all 0.3s ease;
}

.sidebar a:hover {
  background: #7CFC00;
  color: #000;
  transform: scale(1.05);
}

/* CONTENIDO PRINCIPAL */
.main-content {
  margin-left: 240px;
  padding: 20px;
  width: calc(100% - 240px);
}

/* HERO PORTADA */
.hero {
  height: 50vh;
  background-image: url('images.jpeg');
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
  position: relative;
  border-radius: 10px;
  margin-bottom: 20px;
}

.hero::after {
  content: "";
  position: absolute;
  top:0; left:0; right:0; bottom:0;
  background: rgba(0,0,0,0.45);
  border-radius: 10px;
}

.hero-content {
  position: relative;
  z-index: 1;
}

.hero h1 {
  font-size: 40px;
  margin-bottom: 10px;
}

.hero p {
  font-size: 18px;
}

/* TARJETAS */
.card {
  background:white;
  padding:25px;
  margin:20px 0;
  border-radius:10px;
  box-shadow:0 4px 10px rgba(0,0,0,0.1);
  transition:all 0.3s ease;
  opacity:0;
  transform:translateY(30px);
}

.card.show {
  opacity:1;
  transform:translateY(0);
}

.card:hover {
  transform:translateY(-8px);
  box-shadow:0 10px 25px rgba(0,0,0,0.2);
}

/* GRID TEMAS */
.temas {
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:25px;
  margin-top:30px;
}

.tema {
  background:white;
  padding:25px;
  border-radius:12px;
  text-align:center;
  box-shadow:0 4px 10px rgba(0,0,0,0.1);
  transition:all 0.35s ease;
  cursor:pointer;
  text-decoration:none;
  color:#333;
}

.tema:hover {
  transform:translateY(-10px) scale(1.05);
  box-shadow:0 12px 25px rgba(0,0,0,0.25);
}

.tema i {
  font-size:40px;
  margin-bottom:15px;
  color:#2e8b57;
}

.tema h3 {
  margin-bottom:10px;
}

/* FOOTER */
footer {
  background:#111;
  color:white;
  text-align:center;
  padding:20px;
  margin-top:30px;
}

/* RESPONSIVE */
@media(max-width: 768px) {
  body {
    flex-direction: column;
  }
  .sidebar {
    width: 100%;
    position: relative;
  }
  .main-content {
    margin-left: 0;
    width: 100%;
  }
}
</style>

</head>
<body>

<!-- SIDEBAR LATERAL -->
<div class="sidebar">
  <h2>Índice</h2>
  <a href="index.html">Inicio</a>
  <a href="contaminacion.html">Contaminación ambiental</a>
  <a href="residuos.html">Residuos informáticos</a>
  <a href="obsolescencia.html">Obsolescencia programada</a>
  <a href="informatica-ecologica.html">Informática ecológica</a>
  <a href="referencias.html">Referencias</a>
</div>

<!-- CONTENIDO PRINCIPAL -->
<div class="main-content">

  <div class="hero">
    <div class="hero-content">
      <h1>🌍 Informática y Protección Medioambiental</h1>
      <p>El impacto de la tecnología en el planeta</p>
    </div>
  </div>

  <section class="card">
    <h2>Introducción</h2>
    <p>
      La informática forma parte de nuestra vida diaria. Utilizamos ordenadores, teléfonos móviles y muchos dispositivos electrónicos para estudiar, trabajar y comunicarnos.
    </p>
    <p>
      Sin embargo, la fabricación de estos dispositivos requiere recursos naturales y energía, generando contaminación y residuos tecnológicos.
    </p>
  </section>

  <section class="card">
    <h2>Temas del proyecto</h2>
    <div class="temas">
      <a class="tema" href="contaminacion.md">
        <i class="fa-solid fa-industry"></i>
        <h3>Contaminación ambiental</h3>
        <p>Impacto de las actividades humanas y tecnológicas.</p>
      </a>
      <a class="tema" href="residuos.md">
        <i class="fa-solid fa-computer"></i>
        <h3>Residuos informáticos</h3>
        <p>Dispositivos electrónicos desechados que generan contaminación.</p>
      </a>
      <a class="tema" href="obsolescencia.md">
        <i class="fa-solid fa-hourglass-half"></i>
        <h3>Obsolescencia programada</h3>
        <p>Productos diseñados para durar menos tiempo.</p>
      </a>
      <a class="tema" href="informatica-ecologica.md">
        <i class="fa-solid fa-leaf"></i>
        <h3>Informática ecológica</h3>
        <p>Tecnología eficiente y sostenible.</p>
      </a>
    </div>
  </section>

</div>

<footer>
  <p>Proyecto de Informática y Medio Ambiente</p>
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
