<template>
  <div class="header-container bg-dark text-white py-3 px-5 d-flex justify-content-between align-items-center">
    <img src="/assets/img/LOGO-SMK4 1.png" class="school-logo me-3" />
    <div class="flex-grow-1 text-center">
      <h1 class="school-title">
        {{ title }} <span class="school-subtitle">{{ subtitle }}</span>
      </h1>
      <p class="school-address">{{ address }}</p>
    </div>
    <!-- <img src="/assets/img/logo 1.png" alt="Kota Tasik Logo" class="city-logo" /> -->

    <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link text-white" href="/">Beranda</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="/pages/profil">Profil</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="/pages/ekstrakurikuler">Ekstrakurikuler</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="/pages/galeri">Galeri</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white" href="/pages/feedback">Feedback</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <img src="/assets/img/logo 1.png" alt="Kota Tasik Logo" class="city-logo" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "SMKN 4",
      subtitle: "Tasikmalaya",
      address: "Jln. Depok, Sukamenak, Purbartau, Kota Tasikmalaya, 46196",
      logoLeft: "/path/to/smkn-logo.png",
      logoRight: "/path/to/kota-logo.png",
    };
  },
};
</script>

<style>
@font-face {
  font-family: "Font";
  src: url("/assets/style/04B_30__.TTF") format("truetype");
}
.header-container {
  font-family: "Arial", sans-serif;
}

.school-logo,
.city-logo {
  height: 70px;
}

.school-title {
  font-family: "Font", cursive;
  font-size: 2.5rem;
  font-weight: bold;
  text-align: center;
}

.school-subtitle {
  font-style: italic;
}

.school-address {
  margin-top: 5px;
  font-size: 1rem;
  text-align: center;
}
</style>
