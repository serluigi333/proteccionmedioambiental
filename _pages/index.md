---
title: Contaminación ambiental
layout: default
---
# Contaminación ambiental

<style>
  /* --- ANIMACIONES AVANZADAS --- */
  
  /* Animación de aparición desde abajo */
  @keyframes fadeInUp {
    0% { opacity: 0; transform: translateY(30px); }
    100% { opacity: 1; transform: translateY(0); }
  }

  /* Animación de fondo en movimiento continuo */
  @keyframes gradientBG {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  /* Clases para aplicar las animaciones en orden (cascada) */
  .retraso-1 { animation: fadeInUp 0.8s ease-out forwards; }
  .retraso-2 { opacity: 0; animation: fadeInUp 0.8s ease-out 0.3s forwards; }
  .retraso-3 { opacity: 0; animation: fadeInUp 0.8s ease-out 0.6s forwards; }
  .retraso-4 { opacity: 0; animation: fadeInUp 0.8s ease-out 0.9s forwards; }

  /* --- ESTILOS DE LOS ELEMENTOS --- */

  /* Caja de introducción con fondo animado */
  .caja-animada {
    background: linear-gradient(-45deg, #e0f2f1, #b2dfdb, #80cbc4, #e8f5e9);
    background-size: 400% 400%;
    animation: gradientBG 10s ease infinite, fadeInUp 0.8s ease-out forwards;
    padding: 20px;
    border-radius: 12px;
    border-left: 6px solid #00695c;
    color: #333;
    font-size: 1.1em;
    margin: 20px 0;
    box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  }

  /* Estilo avanzado para la tabla (para que no falle en GitHub) */
  table {
    width: 100%;
    border-collapse: collapse;
    margin: 25px 0;
    font-size: 0.95em;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.05);
    border-radius: 8px;
    overflow: hidden;
  }
  thead tr {
    background-color: #00695c;
    color: #ffffff;
    text-align: left;
  }
  th, td {
    padding: 12px 15px;
  }
  tbody tr {
    border-bottom: 1px solid #dddddd;
    transition: background-color 0.3s ease;
  }
  tbody tr:nth-of-type(even) {
    background-color: #f3f3f3;
  }
  tbody tr:hover {
    background-color: #e0f2f1; /* Resalta la fila al pasar el ratón */
  }

  /* Grid para los botones del índice */
  .grid-indice {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
    margin-top: 20px;
  }

  /* Botones con efecto de brillo/resplandor */
  .btn-magico {
    display: block;
    padding: 15px;
    background-color: #26a69a;
    color: white !important;
    text-decoration: none;
    border-radius: 10px;
    font-weight: bold;
    text-align: center;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    position: relative;
    overflow: hidden;
  }
  
  .btn-magico:hover {
    transform: translateY(-5px) scale(1.02);
    background-color: #00897b;
    box-shadow: 0 10px 20px rgba(0, 137, 123, 0.4);
  }
</style>

<div markdown="1">

<div class="retraso-1">

# Proyecto 1: Protección Medioambiental

<div class="caja-animada">
  <strong>Objetivo del Proyecto:</strong> En este espacio analizaremos el impacto crítico de la tecnología en nuestro planeta. Exploraremos qué es la contaminación ambiental, cómo nos ahogan los residuos informáticos, la trampa de la obsolescencia programada y cómo la informática ecológica es nuestra mejor herramienta para un futuro sostenible.
</div>

</div>

<div class="retraso-2" markdown="1">

## Criterios de Calificación


| Nº | Criterio | Puntuación |
|----|----------|------------|
| 1 | Estructura completa: **Título, Índice, Referencias y Autores** | 1 punto |
| 2 | Mínimo **4 imágenes** | 1 punto |
| 3 | Desarrollo correcto de los contenidos | 1 punto por apartado |
| 4 | Uso de características de **Markdown no vistas en clase** | 1 punto |
| 5 | Trabajo colaborativo en grupos diferentes | Obligatorio |

</div>

<div class="retraso-3" markdown="1">

---

## Índice Secundario

Selecciona el apartado que deseas explorar:

<div class="grid-indice retraso-4">
  <a href="contaminacion.html" class="btn-magico">1. ¿Qué es la contaminación ambiental?</a>
  <a href="residuos.html" class="btn-magico">2. Residuos informáticos</a>
  <a href="obsolescencia.html" class="btn-magico">3. Obsolescencia programada</a>
  <a href="ecologica.html" class="btn-magico">4. Informática ecológica</a>
  <a href="referencias_autores.html" class="btn-magico">5. Referencias y Autores</a>
</div>

---

</div>
</div>
