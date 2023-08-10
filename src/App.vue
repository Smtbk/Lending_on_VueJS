<template>
  <nav class="navbar navbar-expand-lg fixed-top navbar-light px-3">
    <div class="container-fluid">
      <a class="navbar-brand p-0 m-0">
        <img src="../src/assets/logo.png">
      </a>
      
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto" role="tablist">
          <li class="nav-item" role="presentation">
            <router-link class="nav-link" to="/">Главная</router-link>
          </li>
          <li class="nav-item" role="presentation">
            <router-link class="nav-link" to="/about">О нас</router-link>
          </li>
          <li class="nav-item" role="presentation">
            <router-link class="nav-link" to="/menu">Меню</router-link>
          </li>
          <li class="nav-item" role="presentation">
            <router-link class="nav-link" to="/reservation">Забронировать столик</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/contacts">Контакты</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  
  <router-view/>
  
  <div>
    <img src="../src/assets/yoki_lent.png" class="d-block w-100">
  </div>
  
  <footer>
    <section class="footer p-3">
      <div class="container">
        <div class="row">
          <div class="footer-icons">
            <a class="m-1" href="#"><i class="bi bi-facebook"></i></a>
            <a class="m-1" href="#"><i class="bi bi-youtube"></i></a>
            <a class="m-1" href="#"><i class="bi bi-telegram"></i></a>
            <a class="m-1" href="#"><i class="bi bi-whatsapp"></i></a>
          </div>
        </div>
      </div>
    </section>
  </footer>
  
</template>

<style>
@import "~bootstrap/dist/css/bootstrap.css";
@import "~bootstrap-icons";
@import "@fontsource/montserrat";

.navbar {
  background-color: #F6F6F6;
}

.nav-link {
  font-size: 21px;
  color: #101010;
  font-family: 'Montserrat';
  font-weight: 300; 
  line-height: 1.2;
  margin-top: 10px; 
  margin-bottom: 15px;
}

.nav-link:hover {
  color: #FFE239;
  font-weight: 900;
}

.nav-link:focus {
  color: #FFE239;
}

body {
  background-color: #202020;
}

footer a {
  color: grey;
  font-size: 2rem;
}

footer a:hover {
  color: #fFE239;
}
</style>
