<script setup>
import hamburguesa from './assets/images/hamburguesa.jpg'
import alitas from './assets/images/alitas.jpg'
import boneless from './assets/images/boneless.jpg'
import Frase3 from './assets/images/Frase3.jpg'
</script>

<template>
  <div>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-danger px-4">
      <div class="container-fluid">
        <a class="navbar-brand fw-bold" >Postres Galicia 💫</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#menuNav">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="menuNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item"><a class="nav-link" href="contacto.html">Contacto</a></li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Hero -->
    <section class="bg-light text-center py-5 hero-section">
      <div class="container">
        <h1 class="display-4 fw-bold">¡Sabor que conquista!</h1>
        <p class="lead">Una comida bien equilibrada es como un poema al desarrollo de la vida</p>
        <a href="menu.html" class="btn btn-warning btn-lg mt-3">¡Explora el menú y pide lo que se te antoje! 🤤</a>
      </div>
    </section>

    <!-- Carrusel automático sin controles -->
<div id="carouselFood" class="carousel slide container my-4" data-bs-ride="carousel" data-bs-interval="4000">
  <div class="carousel-inner rounded shadow overflow-hidden" style="max-height: 400px;">
    
    <!-- Imagen 1 -->
    <div class="carousel-item active d-flex justify-content-center align-items-center" style="height: 150%;">
      <img :src="Frase3" 
           class="img-fluid rounded" 
           style="object-fit: cover; max-height: 150%; max-width: 150%;" 
           alt="Frase3">
    </div>

 </div>

  <!-- Controles -->
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselFood" data-bs-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselFood" data-bs-slide="next">
    <span class="carousel-control-next-icon"></span>
  </button>
</div>

    <!-- Productos -->
    <section class="container text-center my-5">
      <h2 class="mb-4 text-danger fw-bold">🔥 Lo más vendido</h2>
      <div class="row g-4">
        <!-- Hamburguesa -->
        <div class="col-lg-4 col-md-6">
          <div class="card h-100 shadow-sm border-0">
            <img :src="hamburguesa" class="card-img-top img-fluid" style="height: 220px; object-fit: cover;" alt="Hamburguesa">
            <div class="card-body">
              <h5 class="card-title">Hamburguesa Arrachera</h5>
              <p class="card-text text-danger fw-semibold">$120 MXN</p>
            </div>
          </div>
        </div>
        <!-- Alitas -->
        <div class="col-lg-4 col-md-6">
          <div class="card h-100 shadow-sm border-0">
            <img :src="alitas" class="card-img-top img-fluid" style="height: 220px; object-fit: cover;" alt="Alitas">
            <div class="card-body">
              <h5 class="card-title">Alitas BBQ</h5>
              <p class="card-text text-danger fw-semibold">$75 MXN</p>
            </div>
          </div>
        </div>
        <!-- Boneless -->
        <div class="col-lg-4 col-md-6">
          <div class="card h-100 shadow-sm border-0">
            <img :src="boneless" class="card-img-top img-fluid" style="height: 220px; object-fit: cover;" alt="Boneless">
            <div class="card-body">
              <h5 class="card-title">Boneless BBQ</h5>
              <p class="card-text text-danger fw-semibold">$75 MXN</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Frase -->
    <section class="bg-warning text-center text-dark py-5">
      <div class="container">
        <h3 class="fw-bold">“Una mordida y no podrás parar”</h3>
        <p class="mb-0">Nuestros clientes lo confirman</p>
      </div>
    </section>
    
<!-- Sección de delivery -->
<section class="bg-light py-5 text-center">
  <h2 class="mb-4">¡Encuentra Postres Galicia en tus apps favoritas! 🍰</h2>
  <div class="container">
    <div class="row justify-content-center g-4">

      <!-- Didi -->
      <div class="col-md-4">
        <div class="card border-0 shadow">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRVR1wLMX9LC3Me0EDrxmv9MQQySUyNaNG5sA&s" class="card-img-top" alt="Didi" style="height:120px; object-fit:contain;">
          <div class="card-body">
            <a href="https://www.didiglobal.com/mx/user/tu-usuario" class="btn btn-danger">Ordena ahora</a>
          </div>
        </div>
      </div>

      <!-- Uber Eats -->
      <div class="col-md-4">
        <div class="card border-0 shadow">
          <img src="https://1000marcas.net/wp-content/uploads/2020/10/Uber-Eats-Logo-1.jpg" class="card-img-top" alt="Uber Eats" style="height:120px; object-fit:contain;">
          <div class="card-body">
            <a href="https://www.uber.com/mx/user/tu-usuario" class="btn btn-dark">Pide aquí</a>
          </div>
        </div>
      </div>

      <!-- Rappi -->
      <div class="col-md-4">
        <div class="card border-0 shadow">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSI8KWUT0_ov6pcYBZKYjdeA_RSYRCiWMCn5gUZ3jJgT1DYAq3X" class="card-img-top" alt="Rappi" style="height:120px; object-fit:contain;">
          <div class="card-body">
            <a href="https://www.rappi.com.mx/tu-usuario" class="btn btn-warning">¡Antojo rápido!</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

    <!-- Footer -->
    <footer class="bg-danger text-white text-center py-4 mt-5">
    <p class="mb-2">&copy; 2025 Postres Galicia. Todos los derechos reservados.</p>
</footer>
  </div>
</template>

<style scoped>
    .navbar-brand {
      font-family: 'Pacifico', cursive;
      font-size: 2rem;
      color: white;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
    }
</style>