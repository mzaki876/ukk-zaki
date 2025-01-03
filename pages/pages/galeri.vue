<template>
  <div class="container">
    <h1 class=" text-black text-center rounded-3 p-2 m-3">Galeri Foto</h1>
    <div class="gallery">
      <div class="gallery-item">
        <img src="/assets/img/Snapinsta.app_429985310_412816707961616_315052747710584717_n_1080.jpg" alt="Foto 1" />
      </div>
      <div class="gallery-item">
        <img src="/assets/img/Snapinsta.app_466142987_8883376051756962_388448154772462288_n_1080.jpg" alt="Foto 2" />
      </div>
      <div class="gallery-item">
        <img src="/assets/img/Snapinsta.app_387800960_656393913250648_8034974429035700407_n_1080.jpg" alt="Foto 3" />
      </div>
      <div class="gallery-item">
        <img src="/assets/img/Snapinsta.app_430191575_1117608179273386_7917368729099941873_n_1080.jpg" alt="Foto 4" />
      </div>
      <div class="gallery-item">
        <img src="/assets/img/Snapinsta.app_429830371_773017424361127_1152515408500765180_n_1080.jpg" alt="Foto 5" />
      </div>
      <div class="gallery-item">
        <img src="/assets/img/Snapinsta.app_466098767_484872801267204_4394882842595938193_n_1080.jpg" alt="Foto 6" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  text-align: center;
}

h1 {
  margin-bottom: 20px;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 15px;
  max-width: 900px;
  margin: 0 auto;
}

.gallery-item {
  overflow: hidden;
  position: relative;
}

.gallery-item img {
  width: 100%;
  height: 200px; /* Set height to ensure uniform size */
  object-fit: cover; /* Ensure images maintain aspect ratio without distortion */
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.gallery-item img:hover {
  transform: scale(1.05);
}
</style>
